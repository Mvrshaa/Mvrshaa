<!--- <h1 align="center"></h1> --->
# 👋 Hello! I'm Marsha.

🚀 A researcher at heart, driven by curiosity.</br>
🌱 Expanding my expertise in data science, machine learning, and deep learning.</br>
🔭 Currently immersed in everything and anything Data Science.</br>
🔍 Exploring models, digging into datasets, and loving the process of learning more every day.</br>
👯 Always open to collaborating. Let's brainstorm, build, and grow together in the world of data!.</br>
📫 You can reach me <a href="https://www.linkedin.com/in/marshaa">here</a></br>

### Skills
<!--- ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) --->
<!--- ![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white) --->
<!--- ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) --->
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![R](https://img.shields.io/badge/r-%23276DC3.svg?style=for-the-badge&logo=r&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Power BI](https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=power-bi&logoColor=black)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white) 
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoft-azure&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
<!--- ![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?style=for-the-badge&logo=scipy&logoColor=%white) --->
<!---![mlflow](https://img.shields.io/badge/mlflow-%23d9ead3.svg?style=for-the-badge&logo=numpy&logoColor=blue)
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache%20Spark-FDEE21?style=flat-square&logo=apachespark&logoColor=black)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![Azure](https://img.shields.io/badge/azure-%230072C6.svg?style=for-the-badge&logo=microsoftazure&logoColor=white) --->



### 📊 My GitHub Stats:
# stats_generator.py
import requests

# GitHub username
username = "Mvrshaa"

# Fetch public repos for the user
try:
    response = requests.get(f"https://api.github.com/users/{username}/repos")
    response.raise_for_status()
    repos = response.json()
except requests.exceptions.RequestException as e:
    print(f"Error fetching repos: {e}")
    repos = []

# Calculate top languages
lang_count = {}
for repo in repos:
    lang = repo['language']
    if lang:
        lang_count[lang] = lang_count.get(lang, 0) + 1

top_langs = sorted(lang_count.items(), key=lambda x: x[1], reverse=True)[:5]

print(f"Top 5 languages for {username}:")
for lang, count in top_langs:
    print(f"{lang}: {count} repos")

# Calculate total stars
stars = sum([repo.get('stargazers_count', 0) for repo in repos])
print(f"\nTotal stars across all repos: {stars}")

# Optional: Print total number of repos
print(f"Total public repos: {len(repos)}")



<!---![Marsha's GitHub stats](https://github-readme-stats.vercel.app/api?username=MvrshaaE&show_icons=true&theme=radical)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Mvrshaa&layout=compact&theme=radical)


<!-- [![Marsha's GitHub stats](https://github-readme-stats.vercel.app/api?username=Mvrshaa&theme=synthwave&show_icons=true)](https://github.com/mvrshaa/github-readme-stats)
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Mvrshaa)](https://github.com/Mvrshaa/github-readme-stats) 

<!--- [![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Mvrshaa)](https://github.com/Mvrshaa/github-readme-stats) --->

 
<!--- ## 🏆 GitHub Trophies ---
![](https://github-profile-trophy.vercel.app/?username=Mvrshaa&theme=radical&no-frame=false&no-bg=true&margin-w=4)



