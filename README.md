### Hi there 👋

<!--
**dyns4360/dyns4360** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

### EC2 서버 설정방법
먼저 AWS의 EC2 서비스로 들어가서 "Launch instances" 버튼을 눌러주고<br>
적절한 Name을 입력하고<br>
Application and OS Images에서 "Ubuntu"를 선택해준다.<br>
이미지는 자동으로 선택되는 이미지로 나누도록 한다.<br>
(2024년 03월 18일 기준으로 Ubuntu Server 22.04 LTS가 선택된다)<br>
Instance type은 "t2.micro"를 선택해준다.<br>
아래의 Key pair를 선택하는 곳에서는 이전에 만들어두었던 "KeyForBlingEc2.pem" Key를 선택한다.<br>
키를 만들어둘 당시에 .pem 파일이 다운로드 되는데, 이를 D드라이브 최상위 디렉토리에 나두도록 한다.<br>
아래의 네트워크 설정에서는 "Allow SSH Traffic from Anywhere"를 포함한 모든 설정을 기본으로 나두고,<br>
"Allow HTTPS traffic from the internet"과 "Allow HTTP traffic from the internet" 항목에 체크를 해둔다.<br>
Configure storage도 프리티어가 허용하는 만큼만 사용이 되도록 디폴트 값으로 나둔 후 "Launch instance" 버튼을 누르도록 한다.

