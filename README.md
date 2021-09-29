⚡ Technologies

![JavaScript](https://img.shields.io/badge/-JavaScript-black?style=flat-square&logo=javascript)
![React](https://img.shields.io/badge/-React-black?style=flat-square&logo=react)
![HTML5](https://img.shields.io/badge/-HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/-CSS3-1572B6?style=flat-square&logo=css3)
![MySQL](https://img.shields.io/badge/-MySQL-black?style=flat-square&logo=mysql)
![Git](https://img.shields.io/badge/-Git-black?style=flat-square&logo=git)
![GitHub](https://img.shields.io/badge/-GitHub-181717?style=flat-square&logo=github)

```javascript
import React,{ useState }from 'react';

export default function App() {
  const [input, setInput] = useState("");
  const [data, setData] = useState([]);

  async function handleSearch() {
    try {
      const response = await fetch(`https://api.github.com/users/${input}/repos`);
      const value = await response.json();
      setData(value);
      console.log(data);
    }catch(error) {
      alert(error);
    }
    return (
        <>
            <TextInput
              multiline={false}
              autoCorrect={false}
              onChangeText={setInput}
              placeholder="Username GITHUB"
            />
            <BgSearch onPress={() => {
            handleSearch()
            }}>
        </>
    );
}
```
<a href="https://github.com/renanefrem/portfolio>
  <img align="center" src="https://github-readme-stats.vercel.app/api/pin/?username=renanEfrem&repo=Portfolio&show_icons=true&line_height=27&title_color=8257e5&text_color=8a919a&icon_color=8257e5&bg_color=121214
" alt="Portfolio" />
</a>
