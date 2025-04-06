# Self-hosting
The final part :)

## How I can "Ungooglise"?

The project of my "ungooglisation" come over 2024 because I realized that I no longer use Google and Microsoft services (except for my 365 developer subscription where I only use OneDrive). In fact, I no longer use Google's search engine, I've been using DuckDuckGo for a while, I no longer use Google Chrome either, I use Brave, for everything that is Drive and well I have my NAS and as for Gmail, we'll talk about it more.I built my own ecosystem based on my self-hosted applications and I'm almost independent of the American giants anymore, except for Apple because I use their devices, so I'm required to have an Apple account, otherwise I can't do anything...
For example, here's a case that prompted me to return to Apple's ecosystem and re-enter my own at the same time:
For calendars, I used Google Calendar and for my reminders, Microsoft To-Do. I quickly grew tired of both because I didn't find them convenient enough to use. So I thought, "Why not migrate to iCloud? Plus, it integrates really well with my iPhone/iPad."
So, in the end, Google and Microsoft are no longer of much use except for mass-sapping my personal data to make money.

I try as much as possible to be a digitally sovereign Frenchman because, as Octave Klaba (the founder of OVHcloud) said, "In Europe we are very good but we see ourselves as very small." I find that we depend too much on the Americans, especially in Europe, even though we are doing good things. There is one thing that disappoints me enormously, which is that our health data is entrusted to Microsoft even though it is American, while in France and especially throughout Europe, we have OVHcloud.

Doing this homelab experience is a great thing for me, for my learning and especially for my private life because I have total control over everything that happens there, everything that comes in and goes out. And that's exactly what I wanted.

## Mail management with OVH

With the purchase of my domain name, I also acquired email accounts, and we're going to talk about that. I initially acquired these email accounts for professional reasons, but I eventually realized that I could also use them for personal purposes, notably by gradually replacing all my Google emails with a personal email account that I created using my domain name. I don't just have one email account for personal, professional, or the one I think you already have "me@ngrt.fr," but also for my home lab. Why? Simply because I have accounts that I need to create for my home lab (for example, Uptime Robot for monitoring my public IP address) and be notified in case of a problem. I don't regret this migration at all, because I know that my emails depend on a French third party.
That's not all for emails, because when I created my Apple account in 2021, an iCloud email account was created. I didn't use this email because it was of no use to me and I already had my Google account which was created in 2019. So what should I do? I simply decided to use this email address BUT, it was mainly used for my OVH and Cloudflare account in case of access problems with my email. Everything is centralized in iCloud Mail because I simply configured redirections as well as rules that if an email is intended for me@ngrt.fr, it will be automatically redirected to xxx@icloud.com in a folder created in the name of the mailbox, therefore "me@ngrt.fr". So this allows me to centralize all of this in a single account rather than adding a single account each time and ending up in a big mess, which is impossible.
