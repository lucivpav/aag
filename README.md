# Automata and Grammars utilities

A collection of tools that work with automatons, grammars and formal languages.

## Usage
```
aag [options] input
```
## Example

Transform (non-)deterministic finite automaton into a deterministic finite automaton
```
aag --determinize input
```
### (Non-)deterministic finite automaton syntax

```
NFA  a  b  c   \eps
><A  B  -  C|A  -
B  A  A  A|B  A
<C  C  C  C    -
```

*NFA* automaton name  
*a,b,c* input symbols  
*\eps*  epsilon input symbol  
*A,B,C* states  
*>* indicates the state is a start state  
*<* indicates the state is a final state  
*-* no transition defined for given state and input  
*|* several transitions defined for given state and input  
