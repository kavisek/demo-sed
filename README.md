# Sed Command Tutorial

This is a simple demo of the `sed` command.

## Tutorial

```bash
# Replace first occurrences of 'dragon' with 'unicorn' in the file story.txt
sed 's/dragon/unicorn/' story.txt > story2.txt

# Replace all occurrences of 'dragon' with 'unicorn' in the file story.txt
sed 's/dragon/unicorn/g' story.txt > story2.txt



# Replace the word original with replacement in the stdin text.
# The output is printed to stdout.
echo "original text" | sed 's/original/replacement/'

# Reading files and pipeline results to stdout
cat story.txt | sed 's/dragon/unicorn/g'


# Use the -e paratmeter when you to replace multiple patterns
sed -e 's/old/new/' -e 's/foo/bar/' file.txt


# Use the -r parameter to use extended regular expressions
sed -r 's/(foo|bar)/baz/' file.txt
```