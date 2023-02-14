# News-Webapp using React.js with infinite-scroll
![Preview](https://github.com/KUNJ1311/News-Website/blob/master/public/Screenshot%20(126).png/?raw=true "News")

## Get API KEY

1. Go to [https://newsapi.org/](https://newsapi.org/)
2. Login or create an account
3. Then click on your email-ID from navbar and you will be redirected to your account page and from there you can copy your API KEY.

## Setup project

1. Once you get **API KEY** you need yo add that key in `src/components/News.js` file.

```javascript
// Replace <API KEY> to your key.
    async componentDidMount() {
        let url = "https://newsapi.org/v2/top-headlines?country=in&apiKey=<API KEY>&page=1";
        let data = await fetch(url);
        let parsedData = await data.json()
        console.log(parsedData);
        this.setState({articles: parsedData.articles})
    }
```

2. Run command `npm install` in terminal.
3. Then run the command `npm start` in terminal.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.


