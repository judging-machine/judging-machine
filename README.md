# Name-of-the-Machine
A Machine that thinks.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Are language models seeking the Truth, machine?" \
  | uvx name-of-the-machine \
    --provider-api-key=sk-proj-... \
    --github-token=ghp_... 
```

Or, with a local pip installation:
```bash
pip install name-of-the-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
name-of-the-machine multilogue.txt
```
Or:
```bash
name-of-the-machine multilogue.txt new_turn.txt
```
Or:
```bash
cat multilogue.txt | name-of-the-machine
```
Or:
```bash
cat multilogue.txt | name-of-the-machine > tmp && mv tmp multilogue.txt
```
Or: 
```bash
(cat multilogue.txt; echo:"Theodotos: What do you think, Name-of-the-Machine?") \
  | name-of-the-machine
```
Or:
```bash
cat multilogue.txt new_turn.txt | name-of-the-machine
```
Or:
```bash
cat multilogue.txt new_turn.txt | name-of-the-machine >  tmp && mv tmp multilogue.txt
```
Or, if you have installed other machines:
```bash
cat multilogue.md | name-of-the-machine \
  | summarizing-machine | judging-machine > summary_judgment.md
```

Or use it in your Python code:
```Python
# Python
import name_of_the_machine
```
