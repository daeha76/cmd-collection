### Goto URL (wait)
``` cs
public void NavigateToUrl(string url)
{
    if (_disposed) throw new ObjectDisposedException(nameof(Browser_ops));

    try
    {
        _driver.Navigate().GoToUrl(url);

        // 1.
        _wait.Until(driver => driver.FindElement(By.TagName("body")));

        // 2.
        _wait.Until(driver => driver.FindElement(By.Id("elementId")).Displayed);

        // 3.
        _wait.Until(driver => {
            var element = driver.FindElement(By.CssSelector(".buttonClass"));
            return element != null && element.Enabled;
        });

    }
    catch (Exception ex)
    {
        // URL 이동 실패 시 예외 처리
        Console.WriteLine($"Failed to navigate to URL '{url}': {ex.Message}");
        throw;
    }
}
```
