# Inspiration
public-square-tribus is inspired by, and built according to <a href="https://twitter.com/samecwilliams/status/1347741160165531655">Public Square data Protocol</a> specification proposed by Sam Williams.
Therefore, any post broadcasted using decent.land user interface, it will be over Public Square protocol.

# Is it a DAO?
public-square-tribus will be the only community among tribuses which don't represent a PSC (DAO). Public Square is a free space in the web3.0 world to share posts which exist "forever", permanently broadcasted into Arweave's blockweave.
It was decided to adopt `public-square-tribus` as the official main tribus of decentLand.

# Extended PublicSquare

As mentioned above, public-square-tribus uses PublicSquare data Protocol specification to `post` transactions.

A valid post's transaction must have the following tags:

- `"App-Name", "PublicSquare"`     
- `"Version", "1"`                         
- `"Content-Type", "text/plain"`

  => required tags by PublicSquare protocol

- `"protocol", "decent.land"`
  
  => indicates the use of PublicSquare by decentLand Porotocol

- `"v-protocol", "0.0.1"`
  
  => decentLand protocol's version
  
- `"tribus-name", "public-square"`
  
  => each tribus have a name linked to the existing PSC community. pre-defined for public-square-tribus
  
- `"tribus-id", "null"`
  
  => tribus-id represents the PSC creation transaction ID. pre-defined property for public-square-tribus

- `"username", username`
  
  => the username bound to user's wallet. Unless, it will be `guest_*`

- `"user-id", pub_key`
  
  => user's wallet public key

- `"pfp", pfp`
  
  => transaction ID of 100*100 img. The current version bind profile pictures from predefined pictures array - randomly.

- `"unix-epoch", Date.now()`

# Useful links

**signup:** https://decent.land/signup

**posting instance:** https://decetn.land/post

**public-square-tribus homepage:** https://decent.land/v2/t
