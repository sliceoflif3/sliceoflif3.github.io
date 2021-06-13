

# unordered_set

## Definition

An **unordered_set** is implemented using a hash table where keys are hashed into indices of a hash table so that the insertion is always randomized. All operations on the **unordered_set** takes constant time **O(1)** on an average which can go up to linear time **O(n)** in worst case which depends on the internally used hash function, but practically they perform very well and generally provide a constant time lookup operation. 
The **unordered_set** can contain key of any type – predefined or user-defined data structure but when we define key of type user define the type, we need to specify our comparison function according to which keys will be compared. 

## Construction

```c++
unordered_set<value_type> name;


For example: 

```c++
unordered_set<int> i;
```

## Functions

### Insert

The unordered_set::insert() is a built-in function in C++ STL which is used to insert a new {element} in the unordered_set container. Each element is inserted only if it is not equivalent to any other elements already present in the container (elements in an unordered_set have unique values). The insertion is done automatically at the position according to the container’s criterion. This effectively increases the container size by the number of elements inserted.

**Syntax**

```c++
name.insert(value);
```

**Example**

```c++
	for(int i=0;i<5;i++){
	set.insert(i);
}
```

---

### Begin and End

The **unordered_set::begin()** method is a built in function in C++ STL which is used to return an iterator pointing to the first element in the unordered_set container. The unordered_set::end() function is a built-in function in C++ STL which returns an iterator pointing to the past-the-end-element. These iterator does not directly point to an element, rather it points to the location just after the last element.

**Syntax**

```c++
unordered_set_name.begin();
umap_name.end()
```

**Example**

```c++
unordered_set<int>::iterator it beg = set.begin();
unordered_set<int>::iterator it en = set.end();
```

---

### Count

The **unordered_set::count()** function is a built-in function in C++ STL which is used to count occurrences of a particular element in an unordered_set container. As the unordered_set container does not allows to store duplicate elements so this function is generally used to check if an element is present in the container or not. The function returns 1 if the element is present in the container otherwise it returns 0.

**Syntax**

```c++
unordered_set_name.count(element);
```

**Example**

```c++
if(set.count(20)==1)
	cout<<"20 is in the set";
else 
	cout<<"20 is not in the set";
```

---

### Find

The **unordered_set::find()** function is a built-in function in C++ STL which is used to search for an element in the container. It returns an iterator to the element, if found else, it returns an iterator pointing to unordered_set::end().

**Syntax**

```c++
unordered_set_name.find(key);
```

**Example**

```c++
unordered_set<int>::iterator cur = set.find(20);
```

---

### Clear

The **unordered_set::clear()** function is a built-in function in C++ STL which is used to clear an unordered_set container. That is, this function removes all of the elements from an unordered_set and empties it. All of the iterators, pointers, and references to the container are invalidated. This reduces the size of the container to zero.

**Syntax**

```c++
unordered_set_name.clear();
```

**Example**

```c++
set.clear();
```

---











