## 大家好这里是ErgouTree，也可以叫我树上的二狗  
### （基本全平台同名）  
*本人就读于河北师范大学，软件工程专业，保真的弱，毫无技术那种*  

<!DOCTYPE html>
<html lang="en">

<body>
  <div id="info-container">
    <p id="greeting"></p>
    <p id="time"></p>
    <p id="ip-address"></p>
    <p id="browser-info"></p>
    <p id="system-info"></p>
  </div>
  <script>
    // 获取当前时间并显示
    function displayTime() {
      const now = new Date();
      const hours = now.getHours();
      const minutes = now.getMinutes();
      const seconds = now.getSeconds();
      const timeString = `${hours}:${minutes}:${seconds}`;
      document.getElementById('time').innerHTML = `当前时间：${timeString}`;
    }
    // 尝试获取IP地址（注意：实际中可能因浏览器限制获取不到准确的，这里只是尝试）
    async function getIPAddress() {
      try {
        const response = await fetch('https://api.ipify.org?format=json');
        const data = await response.json();
        document.getElementById('ip-address').innerHTML = `IP地址：${data.ip}`;
      } catch (error) {
        document.getElementById('ip-address').innerHTML = '好神秘，我不知道你的地址';
      }
    }
    // 获取浏览器信息
    function getBrowserInfo() {
      const userAgent = navigator.userAgent;
      let browserName;
      if (userAgent.indexOf('Firefox') > -1) {
        browserName = 'Firefox';
      } else if (userAgent.indexOf('Chrome') > -1) {
        browserName = 'Chrome';
      } else if (userAgent.indexOf('Safari') > -1) {
        browserName = 'Safari';
      } else {
        browserName = '其他浏览器';
      }
      document.getElementById('browser-info').innerHTML = `浏览器：${browserName}`;
    }
    // 获取操作系统信息
    function getSystemInfo() {
      const userAgent = navigator.userAgent;
      let osName;
      if (userAgent.indexOf('Windows') > -1) {
        osName = 'Windows';
      } else if (userAgent.indexOf('Mac') > -1) {
        osName = 'Mac OS';
      } else if (userAgent.indexOf('Linux') > -1) {
        osName = 'Linux';
      } else if (userAgent.indexOf('Android') > -1) {
        osName = 'Android';
      } else if (userAgent.indexOf('iOS') > -1) {
        osName = 'iOS';
      } else {
        osName = '其他操作系统';
      }
      document.getElementById('system-info').innerHTML = `操作系统：${osName}`;
    }
    // 根据不同时间显示不同问候语
    function setGreeting() {
      const now = new Date();
      const hours = now.getHours();
      let greeting;
      if (hours >= 5 && hours < 12) {
        greeting = '早上好！';
      } else if (hours >= 12 && hours < 18) {
        greeting = '下午好！';
      } else if (hours >= 18 && hours < 24) {
        greeting = '晚上好！';
      } else {
        greeting = '凌晨好！';
      }
      document.getElementById('greeting').innerHTML = greeting;
    }
    // 页面加载完成后执行函数获取并显示信息
    window.onload = function () {
      displayTime();
      getIPAddress();
      getBrowserInfo();
      getSystemInfo();
      setGreeting();
    };
  </script>
</body>

</html>

***
## 技术栈
![imgae.png](pic/DeviconC.png)![imgae.png](pic/LogosCPlusplus.png)![image.png](pic/DeviconJava.png)![image.png](pic/DeviconJavascript.png)![image.png](pic/SkillIconsHtml.png)![image.png](pic/SkillIconsCss.png)![image.png](pic/SkillIconsJquery.png)![image.png](pic/SkillIconsPythonLight.png)![image.png](pic/LogosMysql.png)![image.png](pic/DeviconGit.png)![image.png](pic/SkillIconsDocker.png)![image.png](pic/DeviconPlainRust.png)![image.png](pic/CarbonXml.png)![image.png](pic/DeviconAndroidWordmark.png)![image.png](pic/DeviconMatlab.png)![image.png](pic/SkillIconsLatexLight.png)
***
在这里基本会存放个人上课或者自己制作的项目，还有退役oi人的挣扎））  
是一名galgame玩家，喜欢绘画，可以去Facebook和推特上关注我，搜索ErgouTree，基本全平台同名
***
同时也是一名手绘画师，真得看看我画的祈莉吧
![image.jpg](pic/111.jpg)  
