# Spearbot

# Purpose / Why Is This Useful?
 - the below script primitives, while useful on their own, are primarily useful when composed with each other and other tools to create fully functional, ai powered tools. for example, the first tool is:

### spearbit-analyzer (chatbot)
 - what is this: it's a chatbot that has access to the outputs of the below primitives
 - what can it do: answer questions about the codebase it was fed
    - "find me all public functions in solidity"
    - "what does the documentation say about (some function)?
    - "give me all modifiers used in the codebase"
    - "what is the auth style used in this contract?"

### Script Primitives
- doc - generates documentation of code. optionally uses existing documentation to assist. can output in various forms (html, markdown, plaintext)
- sum - generates hierarchical summaries of code (ie at line, function, class, and file levels). can output in various forms (html, markdown, plaintext)
- emb - generates embeddings of code at various chunking levels (ie at line, function, class, and file levels if possible (class & file levesl likely only possible with gpt4-32k))

### TODO / Improvements:
- [ ] create hierarchical embeddings so that we can use a higher number for k-nearest-neighbor search