<h1>Synopsis</h1>
Since most traditional social media platforms are centralized, the emerging decentralized social media platforms promise a different way of data production and control.
Most importantly, it enables users to have full control over their data with no limits, and that's what <b>decent land</b> will provide.

<h1>decent land as a word</h1>

- <i>"decent" :</i> nodding to decency and decentralization in the same time.
- <i>"land" </i> indicating the sum of tribuses (communities) created over the protocol. 

Therefore <i><b>decent land</i></b> reffers to the hope of creating a decent monetized social network.

<h1>Inspirations</h1>
decent land is hybrid of several ideas and protocols combined into one merger protocol:

<h2>reddit:</h2>
Reddit is a community-determined aggregator of content. It is a social platform where users submit posts that other users 'upvote' or 'downvote' based on if they like it.
it's the self-proclaimed “front page of the internet”


<b>What's insipred from reddit?</b>


inspired features are:

- communities as forums
- subreddits
- lot of subjects discussions: philosophy, science, technology,politics, etecera.
- karma

decent land will try to fix:
- skeptical fan base and the Reddit system's negative feedback option
- community centralization: owned by admins
- classifying users basing on their Karma regardless their content
- unclear rules to join a community or to guarantee admin's allow on posts sharing

<h2>KarmaDAO:</h2>

According to Andrew Lee Medium <a href="https://andrwlee.medium.com/announcing-karma-dao-first-ever-token-permissioned-networking-chat-group-on-telegram-5feab7a54def">article</a>, Karma DAO is the first <i>token-permissioned networking chat group on Telegram</i> based on Ethereum blockchain.

<b>What's insipred from karmaDAO?</b>

inspired features are:

- Token-Permissioned DAO
- decentralized social network
- Community Ownership Economy

decent land will try to fix:
- the act of using centralised third party in DAO's core Protocol: Telegram
- User experience
- Protocol's non unification
- Permanent archiving of user's content

<h2>Public Square Protocol</h2>
After Twitter suspend of Trump's account POTUS, and the mysterious privacy policy of Twitter foundation, Sam Williams announced in a <a href="https://twitter.com/samecwilliams/status/1347741160165531655?s=20">tweet</a> about a data protocol for an unbiased public square based on Arweave.

<br><br>
<b>What's insipred from Public Square Protocol?</b>

inspired features are:

- Open protocol, anyone can join the network
- unbiased, rulesless & simple
- permanent storage of discussions
- on-chain user activity

decent land will try to fix

- presence of protocol's dashboard: UI
- monetizing the social protocol by a PSC
- user experience: hardcoded posts


<h1>decent land protocol structure</h1>

According the the pros and cons mentioned above, decent land will be a "better" hybrid built ***totally on-chain***.

<h2>1- Protocol: App-Name</h2>

in intention to create a hierarchical `tags` based protocol, a global tag will be used to identify decentland-related transactions from the network.

> tag: ` "App-Name", "decent.land" `

Also protocol's version will be recorded in another tag. It will follow SamVer versioning

> tag: `"version", "0.0.1"`


<h2>2- Community: Tribus</h2>

communities created over decent land will have a standard hardcoded tag-key defined as `tribus-id` with a tag-value evaluates to the tribus transaction ID

- example: ` "tribus-id", "sew_MAXZIgmyEPzzOTkdAca7SQCL9XTCMfxY3KOE5-M" `

The tribus-id value represents the Community.XYZ profit sharing community creation's transaction ID.

An another key-value pair with a human readable value related tribus tag will be created : ` "tribus-name", "decent-land" `

And if you want to compare it to Reddit, each ` "tribus-name", value ` key-value pair tag is equivalent to a ` /r/communityName `on Reddit.


<b>Tribus Ownership Economy</b>

Before creating a tribus (community), the creator define a minimum held amount of $DLT token by the user to be eligible to post in that community (being a member); regardless of who's the user, his content, or what he's going to post, there is no way to restrict his right to publish in that tribus other than min. held PST token. 

Each tribus will represent a <a href="https://community.xyz">CommunityXYZ</a> community. Therefore, beside DLT token, each tribus will have its own token that can be used to tip and reward their own members.


 **Tribus membership is tradable: *buy to join , sell to leave* **
 
 
 <b>Tribus Structure</b>
 
 Tribus structure will be similar to Merkle Patricia Trie or "Merkle Root" in Ethereum blockchain.
 
keywords:

- Entry trie: Tribus
- sub-node: post in a Tribus
- reply: post's reply(ies)
 
 
<h2>3- Registration </h2>
user register (signup) by sending a transaction to the network with specefic tags using his own wallet.

**Limitations:**

- 1 account per wallet
- username: from 4 to 30 characters
- bio: 0-75 characters
- whitespaces are automatically replaced by a dash "-" if found in the username
- usernames are not unique per account (can be duplicated)

***usernames aren't unique. Although, wallet's public address is used to identify account uniqueness (userID = wallet's address).
Usernames act as "Name" and can be updated anytime as same as bio***

**Tags used to be considered as valid user (at registration):**

- `"App-Name", "decent.land"`
- `"username", ${username}`
- `"version", "0.0.1"`
- `"action", "signup"`
- `"Content-Type", "application/json"`
- `"user-id", ${pub_key}`
- `"unix-epoch", ${userObject["registration_unix_epoch"]}` -- automatically insered by the script



