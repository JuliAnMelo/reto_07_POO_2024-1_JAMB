# reto_07_POO_2024-1_JAMB
## The Restaurant Part III
It was added a iterable, it permits to process ``MenuItem`` objects loops as a method in ``Order`` class: 

```python
class Order:
    """
    """

    def __iter__(self):
        self._index = 0
        return self

    def __next__(self):
        if self._index < len(self.items):
            item = self.items[self._index]
            self._index += 1
            return item
        else:
            raise StopIteration

    """
    """
```

The program works unaltered, to read the complete information, see [The Restaurant](https://github.com/JuliAnMelo/reto_03_POO_2024-1_JAMB?tab=readme-ov-file#the-restaurant) and [The Restaurant Part II](https://github.com/JuliAnMelo/reto_04_POO_2024-1_JAMB#the-restaurant-part-ii)
