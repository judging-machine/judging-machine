# Judging-Machine
A Machine that thinks.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Are language models seeking the Truth, machine?" \
  | uvx judging-machine \
    --provider-api-key=sk-proj-... \
    --github-token=ghp_... 
```

Or, with a local pip installation:
```bash
pip install judging-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
judging-machine multilogue.txt
```
Or:
```bash
judging-machine multilogue.txt new_turn.txt
```
Or:
```bash
cat multilogue.txt | judging-machine
```
Or:
```bash
cat multilogue.txt | judging-machine > tmp && mv tmp multilogue.txt
```
Or: 
```bash
(cat multilogue.txt; echo:"Theodotos: What do you think, Judging-Machine?") \
  | judging-machine
```
Or:
```bash
cat multilogue.txt new_turn.txt | judging-machine
```
Or:
```bash
cat multilogue.txt new_turn.txt | judging-machine >  tmp && mv tmp multilogue.txt
```
Or, if you have installed other machines:
```bash
cat multilogue.md | judging-machine \
  | summarizing-machine | judging-machine > summary_judgment.md
```

Or use it in your Python code:
```Python
# Python
import judging_machine
```
