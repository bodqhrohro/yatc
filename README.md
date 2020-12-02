## Dark times are coming: Google started throttling the PDA version of Google Translate
Possibly it got abused (pretty expected with such a tool, right? ;)), so now 502 errors are returned occasionally. I did some tricks to handle that gracefully, but this tool can no more be considered reliable.

I suggest [translate-shell](https://github.com/soimort/translate-shell) as a replacement; it has better reliablity and more features, as well as more backends. But the downside is an excessively wordy output, like some alternative tools have as well. `yatc` prints only the translation without any fancies.

# yatc
Yet Another Translate Client

This simple bash script was written due to new problems with official Google Translate API (now it's requires to enter a captcha which is not useful in many cases). So I as a long-term user of Opera Mini decided to realise my proposition to use as a backend the dumbphone version of Google Translate as it's pretty simple and uses simple GET requests and HTML responses.

Copy this script to you /usr/bin directory and start using. The command format is much simple:

`yatc en=ru "make a barrel roll"`

Language codes can be found here: [link](https://cloud.google.com/translate/docs/languages)
