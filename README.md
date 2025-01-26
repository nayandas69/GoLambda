# 💻🔥 GoLambda 🔥💻  
**Yo, welcome to the GoLambda fam!**  
This is THE serverless framework you didn’t know you needed. Deploy, trigger, and vibe with your custom functions like a true tech wizard. 🪄✨  

---

## 🧐 What's the Vibe?  
GoLambda is your **BFF** (Best Framework Forever) for:  
- Running code on-demand with **HTTP triggers**. 🌐  
- Automating life with **cron jobs**. ⏰  
- Flexing with **message queue triggers** (async for the win). 📨  
- Keeping it **simple, fast, and Goated**. 🐐  

---

## 🚨 Heads Up, Peeps! 🚨  
This project is **under maintenance** right now. 🛠️💤  
We’re still cooking up all the code magic in the lab. 🧪💻  
**Full code coming soon, so stay tuned** 👀✨  

For now, this repo’s just chilling with the README vibes. 😎✍️ 

---

## 🚀 Features That Slap  
- 🛠️ **Deploy Functions**: Ship your code, and let it thrive.  
- ⚡ **Trigger On-Demand**: HTTP? Queue? Cron? We got you.  
- 🧪 **Sandboxed Execution**: Your code runs safely, we promise. 🛡️  
- 📊 **Logs + Metrics**: Know what’s poppin’ in your framework.  
- 🎨 **Web UI**: (Coming soon) A sleek dashboard for boss-level feels.  

---

## 🛠️ Setup (For Real Ones 💯)  
### Pre-Reqs  
1. **Go** installed – duh. 🟡  
   👉 [Install Go](https://golang.org/dl/)  
2. **Docker** for that sandbox energy. 🐳  
   👉 [Install Docker](https://www.docker.com/)  
3. RabbitMQ to vibe with the queues. 🐰  
   👉 Install it with Docker:  
   ```bash  
   docker run -d --name rabbitmq -p 5672:5672 rabbitmq  
   ```  

---

### Install GoLambda  
1. Clone this masterpiece:  
   ```bash  
   git clone https://github.com/nayandas69/GoLambda.git
   cd GoLambda  
   ```  
2. Set up dependencies:  
   ```bash  
   go mod tidy  
   ```  
3. Run the magic:  
   ```bash  
   go run main.go  
   ```  
4. Test the vibes:  
   ```bash  
   curl http://localhost:8080/ping  
   # Output: {"message":"GoLambda is running!"}  
   ```  

---

## 🔥 How to Use  
### 1️⃣ Deploy a Function  
Send your custom function code via HTTP:  
```bash  
curl -X POST http://localhost:8080/deploy \  
-H "Content-Type: application/json" \  
-d '{  
  "name": "helloWorld",  
  "code": "package main; import \"fmt\"; func Run() { fmt.Println(\"Hello, GoLambda!\") }"  
}'  
```  

### 2️⃣ Trigger a Function  
Make it happen (literally):  
```bash  
curl -X POST http://localhost:8080/trigger/helloWorld  
```  

---

## 🤝 Contribute  
Slide into the codebase and add your magic. Open a PR and make your mark! 🌟  

---

## ⚡ Big Brain Future Plans  
- 🖥️ **Admin Dashboard**: For all the visual learners.  
- 📈 **Better Logs/Metrics**: More data = more flex.  
- 🔒 **Enhanced Security**: Safety first, kiddos.  

---

## 🧑‍💻 Creator Shoutout  
Built with 💖 and way too much coffee ☕ by [Nayan Das](https://github.com/nayandas69). 

---

### ⭐ Star This Repo or Be Square! 😎  
Let’s make GoLambda the GOAT 🐐 of serverless frameworks together.  

---
