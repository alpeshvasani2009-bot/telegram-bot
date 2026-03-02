# telegram-bot
import telebot

TOKEN = "8760600147:AAGBR0tUaPbN73GqOzjk8FaLew710_tqzPA"
bot = telebot.TeleBot(TOKEN)

@bot.message_handler(commands=['start'])
def send_welcome(message):
    bot.reply_to(message, "Hello! Hu tamaro bot chu 🤖")

bot.polling()
