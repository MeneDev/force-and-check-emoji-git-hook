# force-and-check-emoji-git-hook

This is a simple commit-msg hook for git that ensurs that

1. Every commit message begins with an emoji followed by a space
2. Every consecutive sequence of non-space characters surrounded by colons is a valid emoji

## Installation

Copy commit-msg to .git/hooks and make it executable

## Examples

    git commit -m "I forgot the emoji"
    
    > Commit message must start with emoji followed by space


    git commit -m ":sparkels: I always misspell sparkles"
    
    > Commit message contains invalid emoji "sparkels"


    git commit -m ":I: :don:t: :even: :know: what :I:m doing"

    > Commit message contains invalid emoji "don", "even", "I", "know"