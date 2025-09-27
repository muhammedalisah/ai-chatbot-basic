# ai-chatbot-basic
README.md
# AI Chatbot (Basic)
Basit if-else tabanlı terminal chatbot.
def respond(msg):
    msg = msg.lower()
    if "merhaba" in msg or "selam" in msg:
        return "Merhaba! Size nasıl yardımcı olabilirim?"
    if "nasılsın" in msg:
        return "İyiyim, teşekkürler! Sen nasılsın?"
    if "teşekkür" in msg or "sağol" in msg:
        return "Rica ederim!"
    return "Üzgünüm, bunu anlamadım. Başka bir şey sorar mısın?"

if __name__ == "__main__":
    print("Chatbot başlatıldı (çıkmak için 'exit' yazın).")
    while True:
        msg = input("You: ")
        if msg.lower() in ("exit","quit"):
            print("Görüşürüz!")
            break
        print("Bot:", respond(msg))
