```js
class TrieNode {
    children = [];
    endword = false;
}

var Trie = function() {
    this.root = new TrieNode();
};

Trie.prototype.insert = function(word) {
    let curr = this.root;
    for (let cha of word) {
        if (!curr.children[cha]) {
            curr.children[cha] = new TrieNode();
        }
        curr = curr.children[cha];
    }
    curr.endWord = true; // Mark node as end of a word
};

Trie.prototype.search = function(word) {
    let curr = this.root;
    for (let c of word) {
        if (!curr.children[c]) {
            return false;
        }

        curr = curr.children[c];
    }

    return !!curr.endWord;
};

Trie.prototype.startsWith = function(prefix) {
    let curr = this.root;
    for (let c of prefix) {
        if (!curr.children[c]) {
            return false;
        }

        curr = curr.children[c];
    }

    return true;
};
```

# Search Words 

```js
class TrieNode {
    children = {};
    endWord = false;
}

class WordDictionary{
    root = new TrieNode();

    addWord(word) {
        let curr = this.root;

        for (let cha of word) {
            if (!curr.children[cha]) {
                curr.children[cha] = new TrieNode();
            }

            curr = curr.children[cha];
        }

        curr.endWord = true;
    }

    search(word) {
        const recSearch = (index, node) => {
            for (let i = index; i < word.length; i++) {
                const c = word[i]

                if (c === '.') {
                // NOTE: here we are checking if there is a match on 
                    return Object.keys(node.children).some((k) => {
                        return recSearch(i + 1, node.children[k])
                    });
                }

                if (!node.children[c]) {
                    return false;
                }

                node = node.children[c]
            }

            return node.endWord
        }
        
        return recSearch(0, this.root)
    }
}
```