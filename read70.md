#  Reading 35: Dunder Methods

Magic Method

* \__init__
* \__str__
* \__len__

 and a lot more ...
example of __len__:

    class LenSupport:
    def __len__(self):
        return 42
    >>> obj = LenSupport()
    >>> len(obj)
    42

## Object Initialization: \__init__

* Build a constructor once you creat your object

## Object Representation: \__str__, \__repr__

  \__repr__: The “official” string representation of an object.

\__str__: The “informal” or nicely printable string representation.

## Iteration: \__len__, \__getitem__, \__reversed__

    class Account:

    def __len__(self):
        return len(self._transactions)

    def __getitem__(self, position):
        return self._transactions[position]

    >>> len(acc)
    5

## def \__reversed__(self)

    return self[::-1]
    >>> list(reversed(acc))
    [30, -20, 50, -10, 20]

## Operator Overloading for Comparing Accounts: \__eq__, \__lt__

    @total_ordering
    class Account:
    .......

    def __eq__(self, other):
        return self.balance == other.balance

    def __lt__(self, other):
        return self.balance < other.balance
    >>> acc2 > acc
    True

    >>> acc2 < acc
    False

    >>> acc == acc2
    False

## Operator Overloading for Merging Accounts: \__add__  

redefining add fucntion for two different objects.

## Callable Python Objects: \__call__

get back a statment for your comands

    class Account:
    # ... 
    def __call__(self):
        print('Start amount: {}'.format(self.amount))
        print('Transactions: ')
        for transaction in self:
            print(transaction)
        print('\nBalance: {}'.format(self.balance))
        >>> acc = Account('bob', 10)
        >>> acc.add_transaction(20)
        >>> acc.add_transaction(-10)
        >>> acc.add_transaction(50)
        >>> acc.add_transaction(-20)
        >>> acc.add_transaction(30)

        >>> acc()
        Start amount: 10
        Transactions:
        20
        -10
        50
        -20
        30
        Balance: 80

### Context Manager Support and the With Statement: \__enter__, \__exit__

* def: "A context manager is a simple “protocol” (or interface) that your object needs to follow so it can be used with the with statement. Basically all you need to do is add \__enter__ and \__exit__ methods to an object if you want it to function as a context manager."

### Python Generators

    Generator functions are syntactic sugar for writing objects that support the iterator protocol. Generators abstract away much of the boilerplate code needed when writing class-based iterators.
    The yield statement allows you to temporarily suspend execution of a generator function and to pass back values from it.
    Generators start raising StopIteration exceptions after control flow leaves the generator function by any means other than a yield statement.
