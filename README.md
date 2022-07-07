# Build-EVM-from-scratch

To better understand EVM, I build an EVM interpretor from scratch while reading the [Ethereum yellow paper](https://github.com/ethereum/yellowpaper).

# Example Usage

```
$ python main.py 600660070260005360016000f3
[*] EVM starts running
PUSH1 @ pc=0  
stack: [6]    
memory: []    

PUSH1 @ pc=2  
stack: [6, 7] 
memory: []    

MUL @ pc=4    
stack: [42]   
memory: []    

PUSH1 @ pc=5  
stack: [42, 0]
memory: []    

MSTORE8 @ pc=7
stack: []
memory: [42]

PUSH1 @ pc=8
stack: [1]
memory: [42]

PUSH1 @ pc=10
stack: [1, 0]
memory: [42]

RETURN @ pc=12
stack: []
memory: [42]

Output: 0x2a
```
