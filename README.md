# Deliberating-Machine
A machine that deliberates.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Can you deliberate about this, machine?" \
  | uvx deliberating-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install deliberating-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
deliberating-machine -a multilogue.txt
```
Or:
```bash
deliberating-machine multilogue.txt > response.txt
```
Or:
```bash
deliberating-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import deliberating_machine
```
