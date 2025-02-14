# ai.robots.txt

<img src="/assets/images/noai-logo.png" width="100" />

This is an open list of web crawlers associated with AI companies and the training of LLMs to block. We encourage you to contribute to and implement this list on your own site. See [information about the listed crawlers](./table-of-bot-metrics.md) and the [FAQ](https://github.com/ai-robots-txt/ai.robots.txt/blob/main/FAQ.md).

A number of these crawlers have been sourced from [Dark Visitors](https://darkvisitors.com) and we appreciate the ongoing effort they put in to track these crawlers. 

If you'd like to add information about a crawler to the list, please make a pull request with the bot name added to `robots.txt`, `ai.txt`, and any relevant details in `table-of-bot-metrics.md` to help people understand what's crawling.

## Usage

This repository provides the following files:
- `robots.txt`
- `.htaccess`

`robots.txt` implements the Robots Exclusion Protocol ([RFC 9309](https://www.rfc-editor.org/rfc/rfc9309.html)).

`.htaccess` may be used to configure web servers such as [Apache httpd](https://httpd.apache.org/) to return an error page when one of the listed AI crawlers sends a request to the web server.
Note that, as stated in the [httpd documentation](https://httpd.apache.org/docs/current/howto/htaccess.html), more performant methods than an `.htaccess` file exist.


## Contributing

A note about contributing: updates should be added/made to `robots.json`. A GitHub action will then generate the updated `robots.txt`, `table-of-bot-metrics.md`, and `.htaccess`.

## Subscribe to updates

You can subscribe to list updates via RSS/Atom with the releases feed:

```
https://github.com/ai-robots-txt/ai.robots.txt/releases.atom
```

You can subscribe with [Feedly](https://feedly.com/i/subscription/feed/https://github.com/ai-robots-txt/ai.robots.txt/releases.atom), [Inoreader](https://www.inoreader.com/?add_feed=https://github.com/ai-robots-txt/ai.robots.txt/releases.atom), [The Old Reader](https://theoldreader.com/feeds/subscribe?url=https://github.com/ai-robots-txt/ai.robots.txt/releases.atom), [Feedbin](https://feedbin.me/?subscribe=https://github.com/ai-robots-txt/ai.robots.txt/releases.atom), or any other reader app.

Alternatively, you can also subscribe to new releases with your GitHub account by clicking the ⬇️ on "Watch" button at the top of this page, clicking "Custom" and selecting "Releases".

## Report abusive crawlers

If you use [Cloudflare's hard block](https://blog.cloudflare.com/declaring-your-aindependence-block-ai-bots-scrapers-and-crawlers-with-a-single-click) alongside this list, you can report abusive crawlers that don't respect `robots.txt` [here](https://docs.google.com/forms/d/e/1FAIpQLScbUZ2vlNSdcsb8LyTeSF7uLzQI96s0BKGoJ6wQ6ocUFNOKEg/viewform).

## Cloudflare Verified Bots
If you are unable to make use of [Cloudflare's hard block](https://blog.cloudflare.com/declaring-your-aindependence-block-ai-bots-scrapers-and-crawlers-with-a-single-click) and/or have WAF rules that make use of  [Cloudflare's Verified Bots](https://radar.cloudflare.com/traffic/verified-bots) conditions, please note that the following AI web crawlers are considered verified bots by Cloudflare: 
- Amazonbot
- Applebot
- CCBot
- ChatGPT-User
- DuckAssistBot
- GoogleOther
- GPTBot
- OAI-SearchBot
- PerplexityBot
- PetalBot

## Additional resources

- [Blocking Bots with Nginx](https://rknight.me/blog/blocking-bots-with-nginx/) by Robb Knight
- [Blockin' bots.](https://ethanmarcotte.com/wrote/blockin-bots/) by Ethan Marcotte
- [Blocking Bots With 11ty And Apache](https://flamedfury.com/posts/blocking-bots-with-11ty-and-apache/) by fLaMEd fury
- [Blockin' bots on Netlify](https://www.jeremiak.com/blog/block-bots-netlify-edge-functions/) by Jeremia Kimelman
- [Blocking AI web crawlers](https://underlap.org/blocking-ai-web-crawlers) by Glyn Normington
- [Block AI Bots from Crawling Websites Using Robots.txt](https://originality.ai/ai-bot-blocking) by Jonathan Gillham, Originality.AI
