# Assessing your Data Structures Fu
* The purpose of this exercise is to get you used to being quizzed on _Interview Questions_ commonly asked about Data Structures and their implementation in the JavaScript Language.
* Answers to your written questions will be recorded in *Answers.md* 
* This is to be worked on alone but you can use outside resources. You can *reference* any old code you may have, and the React Documentation, however, please refrain from copying and pasting any of your answers. Try and understand the question and put your responses in your own words. Be as thorough as possible when explaining something. 
* **Just a friendly Reminder** Don't fret or get anxious about this, this is a no-pressure assessment that is only going to help guide you here in the near future. This is NOT a pass/fail situation. 

## Questions
1. What are the order of insertions/removals for the following data structures?
   - **Stack** LIFO - Last In, First Out
   - **Queue** FIFO - First In, First Out
2. What is the retrieval time complexity for the following data structures?
   - **Linked List** O(n) - Linear Time - It goes up at the same rate as the size of the dataset.
   - **Hash Table**  O(1) Constant Time - It takes the same amount of time no matter how many elements are in the data set. The hashing time doesn't change with the input or the size of the dataset.
   - **Binary Search Trees**  O(log(n)) - Logarithmic complexity - it goes up log(n) for a dataset of size n. This is much less of an increase than Linear time, but not as good as a time constant such as in a Hash Table, given a data set that is large enough that O(log(n)) is higher than the time required to hash a single input. Smaller datasets would see faster retrieval if implemented as Binary Search Trees.

2. What are some advantages to using a Hash Tables over an array in JavaScript?

If you have a very large data set, the search/insert/retrieval/deletion times are faster with a Hash Table. Any loss of performance due to resizing the table is temporary. 
(They can't be all that great, or Ryan would love them!)

## Challenge
If you take a look at the hash-table.js file you'll notice that it has solution code in it. You'll also notice that if you run the tests, they all pass. Your job is to refactor this hash table solution to use **linked lists** for buckets instead of arrays. You're welcome to add another class to the helper file, following the pattern used with LimitedArray.