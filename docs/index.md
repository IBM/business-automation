<style>
.md-typeset h1 {
  display: none;
}
[data-md-color-scheme="default"] .only-dark { display: none; }
[data-md-color-scheme="slate"] .only-light { display: none; }
</style>

<br/>
<div align="center">
    <a href="https://ibm.github.io/business-automation/" alt="poster">
        <img alt="Scrapling" src="assets/ibm/ibm-blue-logo-transparent-background.png" class="only-light">
        <img alt="Scrapling" src="assets/ibm/ibm-blue-logo-transparent-background.png" class="only-dark">
    </a>
</div>

<h2 align="center"><i>Let's Create</i></h2><br>


## Top Sponsors 

<!-- sponsors -->
<div style="text-align: center;">
    <a href="https://www.thordata.com/?ls=github&lk=github" target="_blank" title="Unblockable proxies and scraping infrastructure, delivering real-time, reliable web data to power AI models and workflows."><img src="https://raw.githubusercontent.com/D4Vinci/Scrapling/main/images/thordata.jpg"></a>
    <a href="https://evomi.com?utm_source=github&utm_medium=banner&utm_campaign=d4vinci-scrapling" target="_blank" title="Evomi is your Swiss Quality Proxy Provider, starting at $0.49/GB"><img src="https://raw.githubusercontent.com/D4Vinci/Scrapling/main/images/evomi.png"></a>
    <a href="https://serpapi.com/?utm_source=scrapling" target="_blank" title="Scrape Google and other search engines with SerpApi"><img src="https://raw.githubusercontent.com/D4Vinci/Scrapling/main/images/SerpApi.png"></a>
    <a href="https://visit.decodo.com/Dy6W0b" target="_blank" title="Try the Most Efficient Residential Proxies for Free"><img src="https://raw.githubusercontent.com/D4Vinci/Scrapling/main/images/decodo.png"></a>
    <a href="https://petrosky.io/d4vinci" target="_blank" title="PetroSky delivers cutting-edge VPS hosting."><img src="https://raw.githubusercontent.com/D4Vinci/Scrapling/main/images/petrosky.png"></a>
    <a href="https://hasdata.com/?utm_source=github&utm_medium=banner&utm_campaign=D4Vinci" target="_blank" title="The web scraping service that actually beats anti-bot systems!"><img src="https://raw.githubusercontent.com/D4Vinci/Scrapling/main/images/hasdata.png"></a>
    <a href="https://proxyempire.io/?ref=scrapling&utm_source=scrapling" target="_blank" title="Collect The Data Your Project Needs with the Best Residential Proxies"><img src="https://raw.githubusercontent.com/D4Vinci/Scrapling/main/images/ProxyEmpire.png"></a>
    <a href="https://hypersolutions.co/?utm_source=github&utm_medium=readme&utm_campaign=scrapling" target="_blank" title="Bot Protection Bypass API for Akamai, DataDome, Incapsula & Kasada"><img src="https://raw.githubusercontent.com/D4Vinci/Scrapling/main/images/HyperSolutions.png"></a>
</div>
<!-- /sponsors -->

<i><sub>Do you want to show your ad here? Click [here](https://github.com/sponsors/D4Vinci/sponsorships?tier_id=435495) and enjoy the rest of the perks!</sub></i>

## Key Features

### Spiders — A Full Crawling Framework
- 🕷️ **Scrapy-like Spider API**: Define spiders with `start_urls`, async `parse` callbacks, and `Request`/`Response` objects.
- ⚡ **Concurrent Crawling**: Configurable concurrency limits, per-domain throttling, and download delays.
- 🔄 **Multi-Session Support**: Unified interface for HTTP requests, and stealthy headless browsers in a single spider — route requests to different sessions by ID.
- 💾 **Pause & Resume**: Checkpoint-based crawl persistence. Press Ctrl+C for a graceful shutdown; restart to resume from where you left off.
- 📡 **Streaming Mode**: Stream scraped items as they arrive via `async for item in spider.stream()` with real-time stats — ideal for UI, pipelines, and long-running crawls.
- 🛡️ **Blocked Request Detection**: Automatic detection and retry of blocked requests with customizable logic.
- 📦 **Built-in Export**: Export results through hooks and your own pipeline or the built-in JSON/JSONL with `result.items.to_json()` / `result.items.to_jsonl()` respectively.

### Advanced Websites Fetching with Session Support
- **HTTP Requests**: Fast and stealthy HTTP requests with the `Fetcher` class. Can impersonate browsers' TLS fingerprint, headers, and use HTTP/3.
- **Dynamic Loading**: Fetch dynamic websites with full browser automation through the `DynamicFetcher` class supporting Playwright's Chromium and Google's Chrome.
- **Anti-bot Bypass**: Advanced stealth capabilities with `StealthyFetcher` and fingerprint spoofing. Can easily bypass all types of Cloudflare's Turnstile/Interstitial with automation.
- **Session Management**: Persistent session support with `FetcherSession`, `StealthySession`, and `DynamicSession` classes for cookie and state management across requests.
- **Proxy Rotation**: Built-in `ProxyRotator` with cyclic or custom rotation strategies across all session types, plus per-request proxy overrides.
- **Domain Blocking**: Block requests to specific domains (and their subdomains) in browser-based fetchers.
- **Async Support**: Complete async support across all fetchers and dedicated async session classes.

### Adaptive Scraping & AI Integration
- 🔄 **Smart Element Tracking**: Relocate elements after website changes using intelligent similarity algorithms.
- 🎯 **Smart Flexible Selection**: CSS selectors, XPath selectors, filter-based search, text search, regex search, and more.
- 🔍 **Find Similar Elements**: Automatically locate elements similar to found elements.
- 🤖 **MCP Server to be used with AI**: Built-in MCP server for AI-assisted Web Scraping and data extraction. The MCP server features powerful, custom capabilities that leverage Scrapling to extract targeted content before passing it to the AI (Claude/Cursor/etc), thereby speeding up operations and reducing costs by minimizing token usage. ([demo video](https://www.youtube.com/watch?v=qyFk3ZNwOxE))

### High-Performance & battle-tested Architecture
- 🚀 **Lightning Fast**: Optimized performance outperforming most Python scraping libraries.
- 🔋 **Memory Efficient**: Optimized data structures and lazy loading for a minimal memory footprint.
- ⚡ **Fast JSON Serialization**: 10x faster than the standard library.
- 🏗️ **Battle tested**: Not only does Scrapling have 92% test coverage and full type hints coverage, but it has been used daily by hundreds of Web Scrapers over the past year.

### Developer/Web Scraper Friendly Experience
- 🎯 **Interactive Web Scraping Shell**: Optional built-in IPython shell with Scrapling integration, shortcuts, and new tools to speed up Web Scraping scripts development, like converting curl requests to Scrapling requests and viewing requests results in your browser.
- 🚀 **Use it directly from the Terminal**: Optionally, you can use Scrapling to scrape a URL without writing a single line of code!
- 🛠️ **Rich Navigation API**: Advanced DOM traversal with parent, sibling, and child navigation methods.
- 🧬 **Enhanced Text Processing**: Built-in regex, cleaning methods, and optimized string operations.
- 📝 **Auto Selector Generation**: Generate robust CSS/XPath selectors for any element.
- 🔌 **Familiar API**: Similar to Scrapy/BeautifulSoup with the same pseudo-elements used in Scrapy/Parsel.
- 📘 **Complete Type Coverage**: Full type hints for excellent IDE support and code completion. The entire codebase is automatically scanned with **PyRight** and **MyPy** with each change.
- 🔋 **Ready Docker image**: With each release, a Docker image containing all browsers is automatically built and pushed.


