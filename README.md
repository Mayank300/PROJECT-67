🚧🚧🚧

**Quirk is no longer being maintained.**

Quirk started as a little thing I made for myself as I started doing CBT. As I got better, I needed Quirk less. But at the same time, lots of other people had discovered Quirk and started picking it up. That meant more bug fixes, more features, and just more work to be done. I really couldn't keep it up well, especially with my main focus at the time (my day job). 

So in order to work on it full time, my brother and I tried to turn it into a company. That way we could continue to develop Quirk as a primary focus, even if we didn't need it anymore. 

For awhile, Quirk was going quite well. Lots of people subscribed, we got backed by [Y Combinator](https://www.ycombinator.com/), and we were growing _very_ quickly. 

Unfortunately, in order for the business to work and for us to pay ourselves, we needed folks to be subscribed for a fair amount of time. But in general, most people fell into three camps: didn't use the app at all (and weren't getting value for what they paid), felt better and then unsubscribed, or didn't feel better but persisted anyway. That meant the business model treated successes as failures and failures as successes. So a future Quirk would need to make people feel worse for longer or otherwise not help people we signed up to help. If the incentives of the business weren't aligned with the people, it would have been naive to assume that we could easily fix it as the organization grew and we held less control. We didn't want to go down that path, so we pivoted the company. 

Anyone who's followed this project will know that we explored multiple paths towards sustainability. Much of it was discussed in the PRs and issues of this repo. We've investigated a completely free model, an indie open source model, a community open source model, a donation model, a pay-up-front model, an ad model, a tele-therapy model, and a subscription model. 

**Quirk (the company) is now Room Service.**

Now-a-days, we're making [Room Service](https://www.roomservice.dev/), which helps folks build multiplayer stuff, like what Figma or Google Docs have. Multiple cursors, CRDTs, sockets, lots of people editing the same thing, that sort of thing. We're still the same commercial entity and such, just making a different product now. If you think multiplayer systems are cool and want to join us, send me an email: `evan @ roomservice . dev`. 

**Make your own Quirk.**

If you like Quirk and want it to continue, feel free to fork it. We'd ask that you change the name to avoid confusion. Just heed our warning, becareful about the way you keep yourself afloat and becareful about your desire to work on this full-time. There's [more of a write up about this here.](https://evanjconrad.com/posts/moral-competence) 

If you want to fork Quirk, you should fork off of [this commit](https://github.com/Flaque/quirk/commit/7a4eabe48414de5edfefcd693e79178120eae142), it's right before we added payments and when the code was the cleanest. 

🚧🚧🚧


---

<p align="left">
<h1 align="center">✨🐙 quirk. </h1>
</p>
<p align="center">
  <a href="https://itunes.apple.com/us/app/quirk-cbt/id1447026451?mt=8">Download iOS</a> • <a href="https://play.google.com/store/apps/details?id=tech.econn.quirk">Download Android</a> • <a href="mailto:humans+github@quirk.fyi">Contact</a> • <a href="https://tinyletter.com/quirk">Newsletter</a>
<br><br>
</p>

Quirk is a crossplatform, GPL-licensed, [Cognitive Behavioral Therapy (CBT)](https://en.wikipedia.org/wiki/Cognitive_behavioral_therapy)
app built in React Native / Expo.

Unlike many CBT apps, it's fairly unbiased in what you use it for; it doesn't ask about you
to do depression-specific CBT exercises. That makes it fairly quick and discreet to use, especially in a public
setting.

![screenshot](https://i.imgur.com/64Cpmpm.png)

## How Quirk Supports Itself

In order for Quirk to support itself, **it charges a small subscription fee.** Currently it's $5.99 / month in the US, which is roughly the cost of a cup of coffee. This helps pay for a full-time developer to make Quirk not-dead and generally good. 

### The Survival Law of Product Design

To understand _why_ we do a subscription, we can look to the Survival Law of Product Design, a fancy term I just made up. When you make a product, whatever keeps that product alive becomes the primary force of design. 

For example, facebook.com is not Facebook's product, facebook.com/business/ads is Facebook's product. Because 0 dollars are made from facebook accounts, only from advertisers that pay to get access to those facebook accounts. The way you keep the lights on ultimately shapes the product you make. 

So if you want to make a good product that helps folks, you should pick a model of sustainability where the financial incentives of the organization are aligned with the individual interests of the users.

After a lot of tries with other models, that ended up being a subscription. In a subscription, the primary metric is retention: are people still using this thing? If retention drops, people cancel their subscription and you no longer get to exist.

The _only_ solid way to have good retention is to create something that is actively useful and good. Similarly, the only way to get any value from CBT is to consistently do it. 

## Contributors

Some amazing folks have helped build the Quirk you see today.

- [@devinroche](https://github.com/devinroche) for setting up translation and stepping up as a core maintainer 🔥
- [@devilcius](https://github.com/devilcius) for the amazing Spanish translation 🇪🇸
- [@idnovic](https://github.com/idnovic) for the amazing German translation 🇩🇪 (and the iPad support!)
- [@kwierbol](https://github.com/kwierbol) for the amazing Polish translation 🇵🇱
- [@Walther](https://github.com/Walther) for the amazing Finnish translation 🇫🇮
- [@Jos512](https://github.com/Jos512) for the amazing Dutch translation 🇳🇱
- [@jinto](https://github.com/jinto) for the amazing Korean translation 🇰🇷
- [@briankung](https://github.com/briankung) for the Chinese 🇨🇳 localization, internationalization support and helping guide the entire translation effort. 🎉
- [@akinariobi](https://github.com/akinariobi) for the Russian translation 🇷🇺 
- [@miguelmf](https://github.com/miguelmf) for the Portugese translation 🇵🇹
- [@comradekingu](https://github.com/comradekingu) for the Norweigan Bokmål translation 🇳🇴
- [@micheleriva](https://github.com/micheleriva) for the Italian translation 🇮🇹
- [@Jolg42](https://github.com/jolg42) for the French translation 🇫🇷
- [@Buricescu](https://github.com/Buricescu) for the Romanian translation 🇷🇴

## Running Locally

Quirk is built on React Native and therefore assumes you have [node](https://nodejs.org/en/) installed.
[Yarn](https://yarnpkg.com/en/) is preferred over NPM as a package manager.

```sh
# clone the project and cd into it
git clone git@github.com:Flaque/quirk.git; cd ./quirk

# copy the sample .env (edit as required)
cp .env.sample .env

# install dependencies
yarn

# start development environment
yarn start
```

You'll then be in the [expo development environment](https://docs.expo.io/versions/latest/).
If you already have XCode installed with a simulator, you can just press `i` to start it.

# Can I help?

Yes !

**If you like the app,** go give it 5 stars! It helps more people find the app.

**If you're a mental health professional,** audit [the descriptions](https://github.com/Flaque/quirk/blob/master/src/locals/en.json) of the cognitive distortions. If you have suggestions, let me know and we'll change stuff!

**If you can draw** and can make digital illustrations of the little blobs, let me know and I'll find a place to stick them in the app!

**If you know a language other than English,** help [us translate the app!](/TRANSLATIONS.md)

# Design

Quirk's goal is to be both inviting and focused. It should be _really_ easy to enter in a thought; people frequently enter these in public settings and need to do it fairly quickly. It also should not cause any increased frustration.

## Design Logic

Quirk is built with two main goals in mind:

- Don't be bloated
- Don't be evil

### Don't be bloated

**Don't include features for one particular condition at the expense of other conditions.** For example, don't couple mood tracking to thought tracking. If a user _has_ to enter a mood in order to track a thought, then the entire app is ruined for people who use it for panic, OCD or another condition where mood isn't the primary focus.

**Don't include non-CBT related treatments without good reason.** No relaxation audio tracks or meditation guides. It's a CBT app, keep it focused on CBT.

**Don't include things that could be better accomplished by another app.** No one needs an in-app diary when a diary works just fine. No one needs an in-app heart rate tracker when a heart rate tracker works just fine.

**Be quick and efficient.** Thoughts shouldn't take 5 minutes to enter and you should be able to skip fields if it's reasonable. Don't let the perfect be the enemy of the good.

### Don't be Evil

**Thoughts are more valuable than passwords, treat them that way.** Most people would rather give over their passwords than their CBT thoughts. They're incredibly private, occasionally involve other people, and frequently are embarrassing.

**Don't have \$200 dollar in app purchases.** I'm looking at you CBT Thought Diary. I get it, developers need to make money. It costs a lot to just keep the app on the app store. But you're preying on vulnerable people. Very few people of rational mind will purposely spend \$200s for a dark mode.

**Don't have dumb notifications.** Scheduling is fine, abusing push notifications so your app has better traffic is scummy and gross.

**Be open.** Not every app has to be open source; it's a hard choice to make. But be clear and obvious within the app about what's going on with the user's data. Don't be sending it to some server without making that clear within the app, especially if it's not providing any extra utility to the user.

**Don't push people to be unhappy.** Do not purposefully or accidentally force people to be unhappy to use their app. Don't force people to state their unhappy in order to access a feature. It's easy for this to sneak up in the design, if a user has to rate their happiness below average in order to access the CBT features, you're asking them to be unhappy to use your app.

**Be extremely cautious about making engagement your core metric.** User engagement is fine to be concerned about. We all want people who need help to be actually engaging in the help. But holy moly becareful about this. You _do not_ want to drive something that is for many people a treatment into a self-perpetuating engagement loop. A ruthless focus on engagement has caused many a product to become skinner boxes. _No one should ever be addicted to your mental health app._

# Engineering Logic

Quirk _must not_ lose user data. The entire point of the app is to record your thoughts, so if you lost them it would be pretty bad. As stated in [one study](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6010839/):

> While an app failure in general can be inconvenient and annoying, it can have serious consequences in the context of mental health apps—someone who has come to rely on an app for emotional support can find a failure “devastating.”

Therefore, data management should be given a higher priority than any other part of the app.

## Taxonomy and Order of Data Failure Cases

The following is a list of extremely _bad_ behaviors and states that could happen in order of severity.

### 1 - Large Scale Data Corruption

All thoughts have been corrupted somehow. For example, the JSON format of every item is wrong. This is put at the top because not only can a user not access the data, but it may spiral out can cause continuing errors forcing the app to be "bricked."

### 2 - Large Scale Data Loss

All thoughts have been deleted without any hope of recovery.

### 3 - Small Scale Data Loss

A small amount of data has been deleted without any hope of recovery.

### 4 - Small Scale Data Corruption

A small amount of data has been corrupted in a recoverable way. The user still has lost data, but the app does not crash, and this is potentially fixable via an update.

Data corruption refers to errors in computer data that occur during writing, reading, storage, transmission, or processing, which introduce unintended changes to the original data. Computer, transmission, and storage systems use a number of measures to provide end-to-end data integrity, or lack of errors.

Data corruption

In general, when data corruption occurs a file containing that data will produce unexpected results when accessed by the system or the related application. Results could range from a minor loss of data to a system crash. For example, if a document file is corrupted, when a person tries to open that file with a document editor they may get an error message, thus the file might not be opened or might open with some of the data corrupted (or in some cases, completely corrupted, leaving the document unintelligible). The adjacent image is a corrupted image file in which most of the information has been lost.

Some types of malware may intentionally corrupt files as part of their payloads, usually by overwriting them with inoperative or garbage code, while a non-malicious virus may also unintentionally corrupt files when it accesses them. If a virus or trojan with this payload method manages to alter files critical to the running of the computer's operating system software or physical hardware, the entire system may be rendered unusable.

Some programs can give a suggestion to repair the file automatically (after the error), and some programs cannot repair it. It depends on the level of corruption, and the built-in functionality of the application to handle the error. There are various causes of the corruption.

Overview
File:Fourteen Second Clip of Corrupted Video.ogv
A video that has been corrupted. Warning: This video contains bright, flashing images.
There are two types of data corruption associated with computer systems: undetected and detected. Undetected data corruption, also known as silent data corruption, results in the most dangerous errors as there is no indication that the data is incorrect. Detected data corruption may be permanent with the loss of data, or may be temporary when some part of the system is able to detect and correct the error; there is no data corruption in the latter case.

Data corruption can occur at any level in a system, from the host to the storage medium. Modern systems attempt to detect corruption at many layers and then recover or correct the corruption; this is almost always successful but very rarely the information arriving in the systems memory is corrupted and can cause unpredictable results.

Data corruption during transmission has a variety of causes. Interruption of data transmission causes information loss. Environmental conditions can interfere with data transmission, especially when dealing with wireless transmission methods. Heavy clouds can block satellite transmissions. Wireless networks are susceptible to interference from devices such as microwave ovens.

Hardware and software failure are the two main causes for data loss. Background radiation, head crashes, and aging or wear of the storage device fall into the former category, while software failure typically occurs due to bugs in the code. Cosmic rays cause most soft errors in DRAM.


# License

Quirk is licensed under the [GPL](https://en.wikipedia.org/wiki/GNU_General_Public_License), which guarantees end users the freedom to study, share, and modify the software.

Note that this license **does not** give free reign to redistribute the name and branding of quirk. So if you'd like to publish your own version, please rename it to avoid end-user confusion.
