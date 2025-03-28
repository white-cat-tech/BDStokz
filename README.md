___
![white-cat-tech_wall](someAssets/remove_bg.png)
___


# BDStokz - Your Ultimate Stock Trading Platform

Welcome to BDStokz, a cutting-edge stock trading platform designed to provide an immersive and efficient trading experience. BDStokz is your one-stop solution for all your stock trading needs, offering a wide range of features to help you make informed decisions and maximize your investment potential.


## About BDStokz

Project [ERD](/Project_ERD_A1_10.pdf) 

BDStokz is a comprehensive stock trading website created as a college project. It allows users to buy and sell stocks, search for specific stock information, monitor the current market situation, and gain insights into the top gainers and losers. With a user-friendly interface and a plethora of tools at your disposal, BDStokz empowers both novice and experienced traders to thrive in the stock market.


**Youtube demo:**


[![Watch the video](https://img.youtube.com/vi/bnvE-kUc1pE/hqdefault.jpg)](https://www.youtube.com/watch?v=bnvE-kUc1pE)


## Key Features

- **Buy and Sell Stocks:** Execute stock trades seamlessly and efficiently, with real-time pricing and order execution.

- **Stock Search:** Find detailed information on any stock, including historical data, charts, and company fundamentals.

- **Market Situation:** Stay updated on the latest market trends and news, ensuring you never miss out on potential opportunities.

- **Top Gainers and Losers:** Identify which stocks are performing exceptionally well or struggling, helping you make informed investment decisions.

- **User-Friendly Interface:** Our intuitive interface ensures that users of all levels can navigate and utilize the platform with ease.
  


## Prerequisites


1. [Oracle 19c Database](https://www.oracle.com/database/)
2. [Node.js](https://nodejs.org)


## How to Get Started

### Get the Repository ###

Clone the repository using following commmand

```bash
git clone https://github.com/white-cat-tech/BdStockz.git
```

 ### Initialize the Database 

1. Connect to the system schema with system username and password using any database management tool

2. Run the following commands
```sql
CREATE USER c##BDStokz IDENTIFIED BY c##BDStokz;    
GRANT CONNECT, RESOURCE, DBA TO c##BDStokz;    
GRANT CREATE SESSION TO c##BDStokz;    
GRANT UNLIMITED TABLESPACE TO c##BDStokz;    
```
3. Reconnect to the newly created schema with the above credentials

4. Run the [megaDump.sql](/SQL%20Dump/megaDump.sql)

### Setting up the environment variables

Create a new file `.env` in the root directory. And the file should have the followings

```bash
DB_USER= YOUR_DB_USER 
DB_PASS= YOUR_DB_PASS
DB_CONNECT_STRING=localhost/orcl
PORT=YOUR_FABOURITE_PORT
JWT_SECRET=YOUR_DIRTY_SECRET
```

If you followed the above then the `.env` should look like this
```bash
PORT = 3000
DB_USER = "C##STOCKDB"
DB_PASS = 13579 
DB_CONNECT_STRING = localhost/orcl 
JWT_SECRET = 4nyth1N9 
```

If you find any error after creating `.env` check whether `dotenv` npm package is installed or not.If it is not installed then 

```bash
npm install dotenv
```
### Initializing the Platform


1. Install the dependencies by running the following command
   
   ```bash
    npm install
   ```

2. Run the backend server which is hosting the frontend by running

   ```bash
    node index.js
   ```

3. Open any browser and go to this link [login](http://localhost:3000/BDStokz/login/login.html)

4. Sign up for a BDStokz account to access all our features or you can use the following dummy credentials
   listed [here](/passwords.md)

5. Start trading!!!


## UI Demonstration
1. Login page
   ![loginPage](someAssets/login_final.png)

2. User Dashboard
   ![userDashboard](someAssets/dasboard.png)

3. Notifications for a user
   ![notifications](someAssets/notification.png)

4. Order List
   ![orderList](someAssets/orderList.png)

5. Succesful placement of order
   ![succesfulPlacement](someAssets/successfulOrder.png)

6. Profit Montoring
   ![profitMontoring](someAssets/profitList.png)

7. Userlist
   ![userList](someAssets/userList.png)

8. User Profile
   ![userProfile](someAssets/userProfile.png)



## Contact Us

Have questions or need assistance? We're here to help. Feel free to contact our support team at [rleyayna@digiwr.com](mailto:rleyayna@digiwr.com).

## Disclaimer

BDStokz is a college project and not intended for actual stock trading. Use it for educational and experimental purposes only.

⭐ <a class="github-button" href="https://github.com/white-cat-tech/BDStokz" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star white-cat-tech/BDStokz on GitHub">Star Our Repository</a>


