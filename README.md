# Rarity Score Template

Implement your own rarity tools using this template.

References:

- https://raritytools.medium.com/ranking-rarity-understanding-rarity-calculation-methods-86ceaeb9b98c
- https://github.com/punkscape/01-rarity-analyser-hackathon

# Needs

Who is this project for and what are their needs?

**Creator**: Person who is making the NFT collection

- Save fees
- Sell collection
- Build community
- Generate hype
- Easily deploy

**Buyer**: People who have bought the nft

- Trade nft
- Buy low
- Sell high
- Collect drops

**Developers**: People who maintain this project

- Clear documentation
- Easily iterate

# Features

- List NFTs from JSON (`data/collection.json`).
- Filter NFTs based on traits, attributes.
- Share NFT for `token_id`: Display rarity score, rarity rank and price (useful for buyers)
- If you deploy using Vercel, changes are deployed automatically.

PS: All webpages are responsive

# How to use

Once you have deployed, you need to change the following for your use:

Using locally:

1. Install packages
```
yarn install
```

2. Change the JSON in `data/collection.json` to your collection.json. If there is an error, raise it as an issue. JSON follows [opensea standards](https://docs.opensea.io/docs/metadata-standards)

3. Change `config/index.js`:
  - `env` : If you're using locally set it to `local`, while deploying set it to `prod`.
  - `LOCAL_API_URL`: Port at which app is running locally. Default value of `http://localhost:3000`
  - `API_URL`: Your vercel URL (when you deploy)
  - `COLLECTION_NAME`: Opensea collection name "OneDayPunks" is an example
  - `COLLECTION_TITLE`: This is for the website title (for SEO)
  - `COLLECTION_DESCRIPTION`: og:description (for SEO)
  - `COLLECTION_IMG_LINK`: og:image for website (for SEO)

[Reference for SEO](https://www.heymeta.com/url/odp-rarity.vercel.app)

4. Running it locally

```
yarn run dev
```

## 🧾 Have I done it before?

Yes, deployed it for:
- [Larp Island](https://larpisland.vercel.app): Took me 1 day, there were issues in metadata/codebase. Fixed all of them. [Transaction Proof](https://etherscan.io/tx/0xe40e628eca5997f5194b371369a64c7e40a12786cb54d9037e853560bfa5a2e5)

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">Every Islander is special, but some are more special than others ... <br><br>Our custom-built open-source rarity tool is now live. Enjoy!<br><br>Hat-tip to buildooor 🛠️ <a href="https://twitter.com/PaiNishant?ref_src=twsrc%5Etfw">@PaiNishant</a> for his code and his guidance and for being a legend 👊<a href="https://t.co/7WytxK1jPH">https://t.co/7WytxK1jPH</a></p>&mdash; Larp Island 🏝 (@larpisland) <a href="https://twitter.com/larpisland/status/1504951132501643268?ref_src=twsrc%5Etfw">March 18, 2022</a></blockquote>

## ▶️ How does it work?

0. Exchange greetings, finish payments.

1. I'll request you for project related details, github creds.

2. Fix the json (if any errors), ensure everything is working and update you along 

3. Tell me any issues you have, can add custom fixes.

4. You get the rarity score for your project, you are extremely happy and leave a tweet that tells everyone how great this service was 🍻

# Stack

- [Next.js](https://nextjs.org/docs)
- [Tailwind CSS](https://tailwindcss.com/)

# Fetching updates

From time to time, I push updates if you want to update your repo with those changes:

```
git remote add upstream https://github.com/0xSunman/nft-rarity.git
git fetch upstream
git merge upstream/main 
```
That'll bring you all the latest changes from the repo.

# Donate

- Solana: 9dPN7gdN9cyGhjiQn5gBU9DQDBxUJafvS873BcW3mpFT

- Ethereum: 0x5A8064F8249D079f02bfb688f4AA86B6b2C65359 

- ENS for donating: nishantpai.eth
