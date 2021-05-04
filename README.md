# Book-Project
Group Project on designing a model that suggests books
The information is scraped from grqaser.org.
The data was cleaned manually. It includes book titles, authors, genres, age range, description and ratings(random). There are two models.
First, the user tells their favorite genre, author, or range. After this, the program filters the data frame and remains only the books based on the user’s inputs. Furthermore, only after this, we choose the book with the highest rating among the remaining books.
In the second one, the model is based on Term Frequency-Inverse Document Frequency (famous as tf-IDF) vectors. It erases words such as 'the', ' and ', 'an' in the English, but in Armenian, and then find similar words in the plots of our books and suggest similar ten books. It is an interesting system that does some calculations with algebraic formulas. 
As this library did not have Armenian stop words in it, I have searched for them and found an example to use it. The program uses the cosine similarity to calculate a numeric quantity that denotes the similarity between two books. Then I use the cosine similarity score since it is independent of magnitude and is relatively easy and fast to calculate cosine(x,y)=x.y⊺||x||.||y||. Overall it is a function that takes an input book name and gives similar books.
