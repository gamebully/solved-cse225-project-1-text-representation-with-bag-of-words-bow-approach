Download Link: https://assignmentchef.com/product/solved-cse225-project-1-text-representation-with-bag-of-words-bow-approach
<br>



Traditional representation methodology of documents in the literature is called Bag of Words (BOW) feature representation.  This representation symbolizes the terms and their corresponding frequencies in a document and it is also named as Vector Space Model (VSM).  Each of these terms in the same document represents an independent dimension in a vector space [1]. The order of words in the sentences is completely lost in bag representation like in sets. This approach mainly emphasizes the frequency of terms. The BOW methodology makes the representation of words simpler in documents; still; it has several problems. One of them is sparse vector representation. This makes the computation expensive especially for real world scenarios, which include big data in textual domains. To address this problem; this project aims to create more a more efficient representation of BOW model by using LinkedLists. Consequently, this project is a programming assignment in C, which aims to build an algorithm based on linked-lists that will build an efficient representation of documents.

Your program needs to open and read text files under the following directories: <em>sport, magazine and health</em>. These are 3 categories of 1150Haber dataset [2]. The number of documents in these categories will be arbitrary. Furthermore, the number of terms in these documents will also be arbitrary.  In other words, the length of these files will be arbitrary.

Your program is expected to do the followings:

<ol>

 <li>(40 points) You need to read all the documents under all the categories. Then you need to build a Master Linked-List (MLL). Each node in this MLL needs to represent a different term in these documents. All the terms in these documents are expected to be in the MLL. There will be cases, the same word occur in different documents, or in the same document. Then, you do not need to add a term into the MLL if it already exists. In other words, be careful about not entering the duplicate records into the MLL. This list needs to be in ascending order.</li>

</ol>




Each record in MLL has 2 pointers: The first of them is for the next record in MLL. The second of them is for the starting record of another Linked-List. This sub LinkedList will represent the documents that contain the term in this record of MLL. Figure-1 shows the structure of MLL.

Master Linked List (MLL) with N nodes (master-linked-list)




Figure.1. Schema of the Master-Linked-List and the Linked-List of Documents




<ol>

 <li> Finding stop words/general words (noise in the documents): You need to find the first 5 general words which occur in all of the categories. In other words, you need to list the terms that are common for all of the categories. The output will be like the following (it needs to be listed in ascending order):</li>

</ol>




Term-1: aaa

Term-2: bbb

Term-3: ccc

Term-4: ddd

Term-5: eee




<ol>

 <li>(30 points) Finding discriminating words: You need to find the first 5 words for each category which occur in that category only, not in other categories. The output will be like the following: (it needs to be listed in ascending order)</li>

</ol>




<table width="259">

 <tbody>

  <tr>

   <td width="86">Category-1</td>

   <td width="86">Category-2</td>

   <td width="86">Category-3</td>

  </tr>

  <tr>

   <td width="86">Term-1</td>

   <td width="86">Term-1a</td>

   <td width="86">Term-1b</td>

  </tr>

  <tr>

   <td width="86">Term-2</td>

   <td width="86">Term-2a</td>

   <td width="86">Term-2b</td>

  </tr>

  <tr>

   <td width="86">Term-3</td>

   <td width="86">Term-3a</td>

   <td width="86">Term-3b</td>

  </tr>

  <tr>

   <td width="86">Term-4</td>

   <td width="86">Term-4a</td>

   <td width="86">Term-4b</td>

  </tr>

  <tr>

   <td width="86">Term-5</td>

   <td width="86">Term-5a</td>

   <td width="86">Term-5b</td>

  </tr>

 </tbody>

</table>




<strong> </strong>

<strong>Important Notes: </strong>

In your demo, we will run your program by <strong>reading arbitrary-length input files. You need to store these files into </strong><strong>linked-lists.  </strong>

<strong> </strong>

<strong>In demo, we will </strong><strong>use different input files and we will check if your program find the correct results or not. We will also check your data structure your design architecture. </strong>

<strong>Of course, other questions based on your implementation and coding structure will be asked you during your demo. These questions will be those kinds of questions that could be answered by only the students who really implement his/her project by himself/herself. </strong>

<strong>The main goal of this project is to be familiar with linked-list. Therefore, if you use arrays instead of linked-lists then you will get zero, unfortunately.</strong>