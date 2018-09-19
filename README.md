1. Obtain the elements of the union between two character vectors.
ans:

vec1 = c(rownames(mtcars[1:15,]))

vec2 = c(rownames(mtcars[10:32,]))

vec12<-union(vec1, vec2) 

vec12



2. Get those elements that are common to both vectors.
ans:

vec1 = c(rownames(mtcars[1:15,]))

vec2 = c(rownames(mtcars[10:32,]))

intersect(vec1,vec2)

3. Get the difference of the elements between two character vectors.
ans:

vec1 = c(rownames(mtcars[1:15,]))

vec2 = c(rownames(mtcars[10:32,]))

setdiff(vec1, vec2)# elements of vec1 which are not present in vec2

setdiff(vec2,vec1)# elements of vec2 which are not present in vec1



4. Test the quality of two character vectors. 
ans:

vec1 = c(rownames(mtcars[1:15,])) 

vec2 = c(rownames(mtcars[11:25,])) 



is.element(vec1,vec2)

identical(vec1,vec2)

setequal(vec1,vec2)

vec1 %in% vec2
