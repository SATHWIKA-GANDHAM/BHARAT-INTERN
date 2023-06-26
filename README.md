# BHARAT-INTERN
!pip install pyspellchecker
!pip install pattern
!pip install autocorrect
!pip install textblob
!pip install textdistance
from spellchecker import SpellChecker
spell=SpellChecker()
misspell_word=input("enter the word")
correct_word=spell.correction(misspell_word)
print(f"correct word for '{misspell_word}' is '{correct_word}' is:")
misspell_word="outo"
suggestions=spell.candidates(misspell_word)
print(f"the suggest words are {suggestions}:")
