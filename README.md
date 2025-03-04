# Nexus NFT Deployment
- Buy VPS di : [t.me/skuycloud](t.me/skuycloud)
- Trakteer buat buy Kopi : https://trakteer.id/brrrskuy/tip `<---`
-----------------
1. First time you can Register `Vercel` : 
https://vercel.com/signup
`Click Hobby,Fill your name,Continue with email,Fill verification code`
- `NOTE : Make sure your Nodejs version 16.0 or Higher`
- `If your Nodejs under v16.0, you can change and Install v20.0 , if Higher you can skip this`

`Delete Nodejs`
```
sudo apt remove --purge -y nodejs
```
`Cleane Configuration`
```
sudo apt autoremove -y
sudo apt autoclean
```
`Install Version Nodejs v20.0`
```
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -
```
```
sudo apt install -y nodejs
```
`Check your version nodejs`
```
node -v
```
2. Create Screen
```
screen -S nexusdev
```
3. Clone Repository
```
git clone https://github.com/nexus-xyz/nexus-nft-example.git
cd nexus-nft-example
```
4. Install Dependencies
```
npm install
```
```
cd frontend
npm install
```
`Move to folder contracts`
```
cd ../contracts
```
```
npm install
```
5. Configure environment
```
cd ../frontend
```
```
nano .env.local
```
`Fill this scipt , if OK you can tap CTRL+S+X`
```
# API and Website URLs
NEXT_PUBLIC_API_URL=http://localhost:3000
NEXT_PUBLIC_WEBSITE_URL=http://localhost:3000

# Firebase Configuration
NEXT_PUBLIC_FIREBASE_API_KEY=your_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_bucket.appspot.com
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id
NEXT_PUBLIC_FIREBASE_MEASUREMENT_ID=your_measurement_id
```
`Back to Contracts file`
```
cd ../contracts
```
```
nano .env
```
`Fill this scipt`
`Note : your_private_key ,Change your Private keys Login in app.Nexus.xyz`
`if OK you can save & close CTRL+S+X`
```
PRIVATE_KEY=your_private_key
NEXUS_RPC_URL=https://rpc.nexus.xyz/http
```
`Back to Frontend file`
```
cd ../frontend
```
4. Install `Vercel` and Configure
```
npm install -g vercel
```
`Next`
```
vercel login
```
`You can see email, click link and put your Code`

![image](https://github.com/user-attachments/assets/0706fb06-6eab-48cc-bfbf-0e38c9e30b7c)

`Next`
```
vercel
```
- Step : Press `Y` , next press `Enter` , next press `N` , Fill project name `nexus` , next press  `Enter` , next press `N`

![image](https://github.com/user-attachments/assets/1efdf981-6a34-4075-8a34-7b7ca87c2d1c)

- Next you can `copy link` in `Production` and go to your Browser `example : https://nexus111-jnpfj6dve-ggclods-projects.vercel.app`

![image](https://github.com/user-attachments/assets/cade7f98-9ee8-43c1-a742-e4dd2a98486f)
- `Connect wallet` , next Fill name and `Deploy Collection`

# Done don`t forget to appreciate coffe for me :D
