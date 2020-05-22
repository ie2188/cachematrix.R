## Put comments here that give an overall description of what your
## functions do

## Write a short comment describing this function

makeCacheMatrix <- function(x = matrix()) {
  #set value of matrix 
  m <- NULL
  set <- function(a) {
    matrix <<- a
    m <<- NULL
  }
  #get the value of matrix 
  get <- function() matrix
  # set inverse of matrix
  setinverse <- function(inverse) m <<- solve
  # get the value of inverse matrix 
  getinverse <- function() m
  list(set = set, get = get,
       setinverse = setinverse,
       getinverse = getinverse)
}

## The function above creates a specific value for the matrix which is then inversed and finally it gives the result 

## Write a short comment describing this function

cacheSolve <- function(x, ...) {
        ## Return a matrix that is the inverse of 'x'
  ## first checks if the inverse has already been calculated 
  matr <- x$getinverse()
  ## if so it gets the inverse and skips inversing 
  if(!is.null(matr)) {
    message("getting cached data")
    return(matr)
  }
  ## otherwise it calsulates the inverse 
  data <- x$get()
  matr <- solve(data, ...)
  matr$setinverse(matr)
  matr
}

## the above fundtion solves the inverse by actually giving us the inverse of the matrix inputed 
