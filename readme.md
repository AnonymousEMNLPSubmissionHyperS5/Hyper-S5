Hello!

Hope you had a nice weekend.
Today, I will upload the exact original code used in the paper, templates used for the datasets, a more legible version, and a working interactive notebook so you can play with and see the models and Hyper-S5 for yourselves.

Please note that we use "real" exact match accuracy (str1 == str2). Papers such as Hyena do not - they repeatedly ask the model the same question using different prompts, and use heavy processing of the models predictions and labels before comparing each other and try to come to a consensus based on whether or not the prediction has the label or not.

There are also bugs in FLAN's codebase that have failed our audit. For example, one of their metrics tries to do a string comparison. Since both objects are strings, the statement returns True and the prediction is counted as correct, regardless of what the strings actually contain.

Therefore, our numbers are not necessarily comparable with other papers. We will have 0's where others may have relatively higher numbers. 

Thank you.
