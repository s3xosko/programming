# current llm training

3 postupne fazy

1. pretraining
klasicky token prediction
trenovaci item = (useknuty text, jeden nasledujuci token)

2. sft = supervised fine tuning
odpovede ake si predstavujeme
trenovaci item = (otazka, odpoved)
generovane ludmi
 - niekomu zaplatim nech mi robi odpovede
 
3. rlhf = reinforcement learning with human feedback 
otazky a viacere odpovede zo skorami
 - dva odpovede, jedna preferovana, jedna nepreferovana, takto je to vacsinou
trenovaci item = (otazka, *(odpoved, skore))
ako ziskam trenovacie data
 - ukazujem ludom otazky a odpovede a nech oskoruju
 - chatgpt da dve odpovede a spyta sa ma kotra sa mi viacej paci
 - ~amazon turk
 - lahsie ziskavat ako data pre stf

