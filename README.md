### CURRENT NEWS, Sep 28: 1.) This script is in a bit of a state of transition, as it no longer fully works with DEXTools following their switch to a different toolbox under-the-hood, but I haven't yet finished adapting it to be fully functional on Astrotools.io or the other sites I want it to work with. I should have it sorted in a few days, hopefully. 

### 2.) I've been unbanned from Telegram, if you knew about that. Still deciding whether I want to stay with that platform, but for the moment, the announcement channel is still [http://t.me/ApopheniaProjects](http://t.me/ApopheniaProjects). If that changes it will be posted here. 

# .

# DYORassistant (formerly "DEXTassistant")

An independently developed userscript bringing new UI features and embedded research tools to popular DEX- &
DeFi-related websites, to give you an edge and help avoid scams. 

# BACKGROUND

## I. Origins

The website  [http://DEXTools.io](http://DEXTools.io) started out as the most popular info explorer
for Uniswap. However, I found that as I explored the information it gave me, I had to do far too
much clicking around to other websites to do my own research on the coins listed. I wanted a quicker
way to gather information and determine which coins might be worth investing in, and more importantly,
which look like scams and should be avoided. So I took all the research I was doing by hand, and coded
an add-on tool that set on top of DEXTools but gave quicker access to all that information, and in
some cases, embedded it right in the page without having to leave DEXTools. Once it was written, it
struck me that this was a good way to lend a hand to beginning traders and newbies, and I decided to
make it available on Github for that purpose.

Since then, script development has begun to shift focus away from DEXTools to other popular sites.
Which I believe are more in keeping with my original intent of helping the beginning traders who need
this most and may not necessarily be in profit yet... traders very much like I was, literally only weeks
ago.

## II. From DextAssistant to DYORassistant: Change of focus and rebranding

As of 1 September 2020, going forward, this script has been rebranded from "DextAssistant" to
"DYORassistant" ("Do Your Own Reasearch" Assistant) to reflect a broader emphasis on helping fledgling
DEX traders research new tokens, rather than just focusing exclusively on enhancing DEXTools. For the
next month, I will be shifting focus to helping new traders by providing information and enhancements
on sites that do not charge the subscription fees that DEXTools will be instituting by the end of September.

The transition will be gradual. But I hope to shift focus before too long completely away from DEXTools, to
whatever tools show the most promising combination of usefulness, accessibility, and value to beginning or
intermediate traders in the months to come. DEXTools is an amazing service run by a great team, and likely
to only get better as it develops; however, I cannot justify volunteering time and development skills for
free to support what now looks like an exclusive service aimed at catering to traders who are already
succesfully enough to be able to afford to pay quite a lot of money for the tools they need. I think it's
terrific that DEXTools is offering an awesome toolset to those traders, I just don't see any reason to
support that myself.

At the same time, I plan on concurrently transitioning away from using DEXTools in my own trading. But I'll
make an effort to support the existing DEXTools-related features, and even continue to add new ones that were
already in the planning stages, for as long as possible.

UPDATE, September 20 2020: Following major under-the-hood changes to DEXTools's UI that are too difficult
to be worth dealing with, some of the script functionality no longer works on that site. The above notes will
be updated shortly. The next major revision of this script will bring full functionality to other sites.

# DISCLAIMER

## TO BE READ IN A STERN, GRUFF VOICE:

Despite my efforts to give it an easy-to-understand GUI, this is an advanced tool for technically
advanced traders.

If you are trading on Uniswap or other DEXs, you need to have a certain level of general knowledge in
order to avoid the high risks, and I'm not going to enable anyone to jump in and lose money. If there's
anything in this you don't understand, then you probably shouldn't be trading on Uniswap yet, so this
tool is not for you.

What's more, as this is under active development, you may find bugs, though I try hard to avoid that.

## Support? Support is for _closers_.

As I'm sharing this for free, I won't give you any support or any guarantees, and if you choose to use
it I don't owe you anything for any reason. It's presented as-is, use it only at your own risk. What
you see is what you get. If you have questions you'll have to do your own research and figure out the
answers yourself. I'm grouchy, don't bother me.

## The murky depths from whence this came

This is an independent project that bubbled up out of a single developer's needs. It's not affiliated
with DEXTools.io or its development team in any way, please *never bother them with questions about it*.

## In not so many words:

Essentially, YOU'RE ON YOUR OWN with this.

Do you think Indiana Jones needed someone holding his hand? No, never. When you're fighting for your
life in a remote jungle or far-flung desert outpost, there's no support, no instruction manual, no second
chances... just your own ingenuity, will to live, and the rich rewards that will come if you can figure
out on your own how to succeed.

As of right now, _that is your life._

(Metaphorically speaking.)

Enjoy!

# INSTRUCTIONS

## Installation

This script *requires a browser plugin that allows you to install and manage user scripts, such as
Greasemonkey, Tampermonkey, or Violentmonkey.* I chose to go with a userscript instead of a browser plugin
because it would allow the code to remain 100% open source and cross-platform.

(Here's where you need to bring a little knowledge to the table. If you're unfamiliar with userscripts or
Tampermonkey, Greasemonkey, Violentmonkey, etc, you should educate yourself from a page like
[https://simply-how.com/enhance-and-fine-tune-any-web-page-the-complete-user-scripts-guide](https://simply-how.com/enhance-and-fine-tune-any-web-page-the-complete-user-scripts-guide)
before you try to use this. BTW I use Tampermonkey [https://www.tampermonkey.net/](https://www.tampermonkey.net/)
myself, on Firefox, Brave, and Chrome, so I know for sure that this script works with that. But you'll
need to decide for yourself which userscript manager is right for you. Consult your doctor.)

*BONUS!* For users that already have a userscript manager extension installed in their browser, you can
install DextAssistant simply by clicking this link: [https://github.com/ApopheniaPays/dextassistant/raw/master/dextAssistant.user.js](https://github.com/ApopheniaPays/dextassistant/raw/master/dextAssistant.user.js).

This script is also hosted at [https://openuserjs.org/scripts/ApopheniaPays/DextAssistant](https://openuserjs.org/scripts/ApopheniaPays/DextAssistant)
for one-click install if you prefer to get a minified version. Supposedly that will stay current as I update
it here, but I haven't checked.

## Features

Global enhancements (currently works on DEXTools.io, Astrotools.io, Trendering.com, Etherscan.io, and Unitradebeta.com):

1.) In any table that has a header row, columns are now sortable.

2.) Ethereum addresses in table columns (indicated by links to Etherscan.io address pages) can be filtered to show only
the rows for that address.

3.) Any links to Etherscan.io now also have a button added to look that address up on Zerion. Ethereum addresses
are color coded to make repeated transactions from the same address more noticeable in tables.

### NOTE: as of 2020 sep 20, not all features listed below may work on DEXTools.io anymore, due to radical
under-the-hood changes to how DEXTools displays information. Most basic functionality has been restored, but not
all. This is the last version of this script that any features are guaranteed to work on DEXTools.

DEXTools.io enhancements:

1.) The most prominent addition is a new icon under the Pool Explorer's Actions column, which opens a
"research assistant" popup that will allow you to view data from other websites pertaining to the token Name,
Contract Address, and Uniswap.info Pair Address for the token on that row. Next to the Contract addresses you
will see a little circled arrow that will show you Google search results for those contract addresses, embedded
right in the popup, when you hover your mouse over it.

2.) For tokens with a particularly low DEXT score or which are auto-generated by a lazy website token-generator
script, the distinguished monocle and handlebar mustache on the "research assistant" gear button are replaced
with a "poop" emoji.

3.) Rows in the the Pool Explorer are color-coded to indicate liquidity adds, removes, and new pools. 100%
liquidity removals are now labeled as "rugpull" instead of just "remove", to make sure you know to feel
extra-bitter.

6.) DEXTools "Dark mode" is now supported, because I was too lazy to attempt any real work tonight.

7.) Rather than rely on the various browser plugins' hinky auto-update mechanism, the script adds an unobtrusive
"update available" link to the footer of the screen after a new version has been pushed to this repo, for
convenient one-click upgrading. (Some extremely nerdy people will notice the script phones home to github on page
load. This update check is why.)

As this script makes cosmetic changes only, there's no harm you can do by poking around. Explore it.

## Usage Tips

Ok, if you need to be told how to use this, you probably aren't ready to be doing this kind of trading. But here's my
basic routine for checking out a token and deciding if it's real or a scam: Check an see any the existing search results
for the contract address, check if liquidity is locked, look at the pair explorer and see if there is website/telegram/
discord referenced and look at those to get an impression. Takes no time at all.

Oh, yeah, and, be extra skeptical if the liquidity pool is less than 1000 ETH. I've seen real coins with pools as small as
20 ETH, but I've never (yet) seen a scam with a pool over 1000 ETH.

# KNOWN ISSUES

1.) Right now the list filtering and sorting only acts on existing rows. As new transactions or pools appear, they
come in at the top, exactly as if the list wasn't filtered or sorted. I'll get around to it. Hey, it's an open
source script, you don't like it, fix it yourself.

# FUTURE PLANS
In keeping with this tool's mission of helping beginning and small traders get a leg up, in an upcoming version this userscript
may begin asking for read-only permission to connect to your wallet (exactly as all dApps currently do.) If you hold enough wealth to
qualify for the premium-level subscriptions to some popular websites, such as holding 20k DEXT for DEXTools 2nd-tier subscription
or holding enough TRND to qualify for Trendering's exclusive 300-member telegram, you may be prevented from further use of this
script. If you wish to avoid these restrictions you may wish not to upgrade the script.
