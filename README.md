# Auto Correction Tool

The AI spell checker should be able to do both of those things.

Correct the word: If the AI is confident that it knows the correct spelling of a word, it should correct the word. For example, if the user enters the word "hte" instead of "the," the AI should correct the word to "the."

Give the word which is nearest to it: If the AI is not confident that it knows the correct spelling of a word, it should give the word which is nearest to it in the dictionary. For example, if the user enters the word "hte," the AI might give the suggestion "the" or "htee."

The AI spell checker should be able to make these decisions based on the following criteria:

The frequency of the word in the dictionary: The more frequently a word appears in the dictionary, the more likely it is that the AI is correct in suggesting it.

The similarity of the word to the misspelled word: The more similar a word is to the misspelled word, the more likely it is that the AI is correct in suggesting it.

The context of the word: The context of the word can also be helpful in determining the correct spelling. For example, if the word "hte" appears in a sentence that talks about the letter "h," the AI is more likely to suggest "the" than "htee."

By considering these criteria, the AI spell checker can provide accurate and helpful suggestions for correcting misspelled words.

## Explanation of Code:

1.pyspellchecker library, which is used for spell checking in Python.

2.SpellChecker class provides methods for checking the spelling of words and suggesting corrections.

3.dict_of_autocorrect_words = {}, creates a new dictionary to store the misspelled words and their suggested corrections.

4.For loop iterates through the words in the sentence and checks if they are misspelled. The spell.unknown() method returns a list of words that are not found in the spell checker's dictionary.

5.dict_of_autocorrect_words[i] = spell.correction(i), adds the misspelled word and its suggested correction to the dictionary. The spell.correction() method returns the suggested correction for a misspelled word.

6.temp = text.split(), splits the sentence into a list of words.

7.res = [], creates a new list to store the corrected words.

8.for wrd in temp:, iterates through the words in the list and adds the corrected word to the new list. The corrected word is obtained from the dictionary, if it exists, or the original word is used if it does not exist.

9.res = ' '.join(res), joins the words in the new list into a sentence.

10.Finally prints the corrected sentence.
