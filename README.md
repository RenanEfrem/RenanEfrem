<img src="https://raw.githubusercontent.com/MicaelliMedeiros/micaellimedeiros/master/image/computer-illustration.png" min-width="400px" max-width="400px" width="400px" align="right" alt="Computador">
</p>
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
<p align="left">
  <a href="mailto: renan.efrem56@gmail.com" alt="Gmail">
  <img src="https://img.shields.io/badge/-Gmail-FF0000?style=flat-square&labelColor=FF0000&logo=gmail&logoColor=white&link=renan.efrem56@gmail.com" /></a>
  
  <a href="https://api.whatsapp.com/send?phone=5515991039477" alt="WhatsApp">
  <img src="https://img.shields.io/badge/-WhatsApp-25d366?style=flat-square&labelColor=25d366&logo=whatsapp&logoColor=white&link=https://api.whatsapp.com/send?phone=5515991039477"/></a>

 
</p>  
