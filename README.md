MINI BUDDY - README
===================

WHAT IS THIS?
A tiny demo chatbot I made for you. It is practice code -
a small toy version of the big idea (an AI bot on WhatsApp).
It only talks in the black window on your computer. It does
NOT connect to WhatsApp yet.

HOW TO RUN IT
1. You need Python on your computer. To check, open the
   black window (terminal) and type:  python3 --version
   If you see a version number, you are good!
2. Go to the folder with these files.
3. Type:  python3 bot.py
4. Talk to Mini Buddy! Type "bye" to stop.

HOW IT WORKS (simple words)
- bot.py is the whole bot. Open it in any text app to read it.
- BRAIN is a little list: when you type a word it knows,
  it answers with the matching reply. That is the bot's "tiny brain".
- get_reply() is the part that reads your message and picks an answer.
- main() is the chat loop: it keeps asking "You:" until you type "bye".

TRY CHANGING IT!
Open bot.py and add your own line to BRAIN, like:
    "pizza": "Yum! I love pizza too!",
Save the file, run it again, and type "pizza". You just taught your bot!

NEW FILE: whatsapp_webhook.py - THE WHATSAPP DOOR
This is the code that WOULD let Mini Buddy chat on WhatsApp.
It still needs YOUR 3 setup steps (Meta account, WhatsApp Business
API approval, always-on server). Until then it only PRETENDS:
run it with  python3 whatsapp_webhook.py  (needs: pip install flask)
and it prints what it WOULD send. The secret keys inside are empty
on purpose - never share real keys with anyone, not even me!

FROM DEMO TO REAL WHATSAPP BOT
A real bot needs 3 big pieces (much harder than this demo):
1. A real BRAIN - instead of the BRAIN list, the bot asks a big
   AI (like Muse) for every answer. That needs an AI account and key.
2. A WHATSAPP DOOR - WhatsApp Business API. You apply at Meta's
   developer site, prove who you are, and get permission. This is
   the official way bots talk on WhatsApp.
3. An ALWAYS-ON COMPUTER - a server (a computer on the internet
   that never sleeps) that runs your bot day and night and passes
   messages between WhatsApp and the AI brain.

This demo is step zero: it teaches you how a chatbot thinks.
The WhatsApp door is the hardest part and needs a grown-up's
help with the Meta application.
