<img src="https://github.com/kichkiro/kichkiro/blob/main/assets/banner_cpp_modules.jpg?raw=true" width="100%"/>

# CPP Modules

C++ is a general-purpose programming language created by Bjarne Stroustrup as an extension of the C programming language, or "C with Classes" (source: Wikipedia).

The goal of these modules is to introduce you to Object-Oriented Programming.

This will be the starting point of your C++ journey. 

Many languages are recommended to learn OOP. 

We decided to choose C++ since it’s derived from your old friend C.
 
Because this is a complex language, and in order to keep things simple, your code will comply with the C++98 standard.
 
We are aware modern C++ is way different in a lot of aspects. 

So if you want to become a proficient C++ developer, it’s up to you to go further after the 42 Common Core!

You will discover new concepts step-by-step. 

The exercises will progressively increase in complexity

<details>
<summary><i><b>Project Structure  📂</b></i></summary>

``` js
├── LICENSE
├── README.md
└── project
    ├── cpp_module_00
    │   ├── ex00
    │   │   ├── Makefile
    │   │   └── megaphone.cpp
    │   ├── ex01
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   ├── Contact.hpp
    │   │   │   └── PhoneBook.hpp
    │   │   └── src
    │   │       ├── Contact.cpp
    │   │       ├── main.cpp
    │   │       └── PhoneBook.cpp
    │   ├── ex02
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   └── Account.hpp
    │   │   └── src
    │   │       ├── Account.cpp
    │   │       └── tests.cpp
    │   └── _subject
    │       ├── 19920104_091532.log
    │       └── en.subject.pdf
    ├── cpp_module_01
    │   ├── ex00
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   └── Zombie.hpp
    │   │   └── src
    │   │       ├── main.cpp
    │   │       ├── newZombie.cpp
    │   │       ├── randomChump.cpp
    │   │       └── Zombie.cpp
    │   ├── ex01
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   └── Zombie.hpp
    │   │   └── src
    │   │       ├── main.cpp
    │   │       ├── Zombie.cpp
    │   │       └── zombieHorde.cpp
    │   ├── ex02
    │   │   ├── main.cpp
    │   │   └── Makefile
    │   ├── ex03
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   ├── HumanA.hpp
    │   │   │   ├── HumanB.hpp
    │   │   │   └── Weapon.hpp
    │   │   └── src
    │   │       ├── HumanA.cpp
    │   │       ├── HumanB.cpp
    │   │       ├── main.cpp
    │   │       └── Weapon.cpp
    │   ├── ex04
    │   │   ├── Makefile
    │   │   ├── test.txt
    │   │   ├── test.txt.replace
    │   │   ├── include
    │   │   │   └── replace.hpp
    │   │   └── src
    │   │       └── main.cpp
    │   ├── ex05
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   └── Harl.hpp
    │   │   └── src
    │   │       ├── Harl.cpp
    │   │       └── main.cpp
    │   ├── ex06
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   └── Harl.hpp
    │   │   └── src
    │   │       ├── Harl.cpp
    │   │       └── main.cpp
    │   └── _subject
    │       └── en.subject.pdf
    ├── cpp_module_02
    │   ├── ex00
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   └── Fixed.hpp
    │   │   └── src
    │   │       ├── Fixed.cpp
    │   │       └── main.cpp
    │   ├── ex01
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   └── Fixed.hpp
    │   │   └── src
    │   │       ├── Fixed.cpp
    │   │       └── main.cpp
    │   ├── ex02
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   └── Fixed.hpp
    │   │   └── src
    │   │       ├── Fixed.cpp
    │   │       └── main.cpp
    │   ├── ex03
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   ├── bsp.hpp
    │   │   │   ├── Fixed.hpp
    │   │   │   └── Point.hpp
    │   │   └── src
    │   │       ├── bsp.cpp
    │   │       ├── Fixed.cpp
    │   │       ├── main.cpp
    │   │       └── Point.cpp
    │   └── _subject
    │       └── en.subject.pdf
    ├── cpp_module_03
    │   ├── ex00
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   └── ClapTrap.hpp
    │   │   └── src
    │   │       ├── ClapTrap.cpp
    │   │       └── main.cpp
    │   ├── ex01
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   ├── ClapTrap.hpp
    │   │   │   └── ScavTrap.hpp
    │   │   └── src
    │   │       ├── ClapTrap.cpp
    │   │       ├── main.cpp
    │   │       └── ScavTrap.cpp
    │   ├── ex02
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   ├── ClapTrap.hpp
    │   │   │   ├── FragTrap.hpp
    │   │   │   └── ScavTrap.hpp
    │   │   └── src
    │   │       ├── ClapTrap.cpp
    │   │       ├── FragTrap.cpp
    │   │       ├── main.cpp
    │   │       └── ScavTrap.cpp
    │   ├── ex03
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   ├── ClapTrap.hpp
    │   │   │   ├── DiamondTrap.hpp
    │   │   │   ├── FragTrap.hpp
    │   │   │   └── ScavTrap.hpp
    │   │   └── src
    │   │       ├── ClapTrap.cpp
    │   │       ├── DiamondTrap.cpp
    │   │       ├── FragTrap.cpp
    │   │       ├── main.cpp
    │   │       └── ScavTrap.cpp
    │   └── _subject
    │       └── en.subject.pdf
    ├── cpp_module_04
    │   ├── ex00
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   ├── Animal.hpp
    │   │   │   ├── Cat.hpp
    │   │   │   ├── Dog.hpp
    │   │   │   ├── WrongAnimal.hpp
    │   │   │   └── WrongCat.hpp
    │   │   └── src
    │   │       ├── Animal.cpp
    │   │       ├── Cat.cpp
    │   │       ├── Dog.cpp
    │   │       ├── main.cpp
    │   │       ├── WrongAnimal.cpp
    │   │       └── WrongCat.cpp
    │   ├── ex01
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   ├── Animal.hpp
    │   │   │   ├── Brain.hpp
    │   │   │   ├── Cat.hpp
    │   │   │   ├── Dog.hpp
    │   │   │   ├── WrongAnimal.hpp
    │   │   │   └── WrongCat.hpp
    │   │   └── src
    │   │       ├── Animal.cpp
    │   │       ├── Brain.cpp
    │   │       ├── Cat.cpp
    │   │       ├── Dog.cpp
    │   │       ├── main.cpp
    │   │       ├── WrongAnimal.cpp
    │   │       └── WrongCat.cpp
    │   ├── ex02
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   ├── AAnimal.hpp
    │   │   │   ├── Brain.hpp
    │   │   │   ├── Cat.hpp
    │   │   │   ├── Dog.hpp
    │   │   │   ├── WrongAnimal.hpp
    │   │   │   └── WrongCat.hpp
    │   │   └── src
    │   │       ├── AAnimal.cpp
    │   │       ├── Brain.cpp
    │   │       ├── Cat.cpp
    │   │       ├── Dog.cpp
    │   │       ├── main.cpp
    │   │       ├── WrongAnimal.cpp
    │   │       └── WrongCat.cpp
    │   ├── ex03
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   ├── AMateria.hpp
    │   │   │   ├── Character.hpp
    │   │   │   ├── Cure.hpp
    │   │   │   ├── Ice.hpp
    │   │   │   ├── ICharacter.hpp
    │   │   │   ├── IMateriaSource.hpp
    │   │   │   └── MateriaSource.hpp
    │   │   └── src
    │   │       ├── AMateria.cpp
    │   │       ├── Character.cpp
    │   │       ├── Cure.cpp
    │   │       ├── Ice.cpp
    │   │       ├── ICharacter.cpp
    │   │       ├── IMateriaSource.cpp
    │   │       ├── main.cpp
    │   │       └── MateriaSource.cpp
    │   └── _subject
    │       └── en.subject.pdf
    ├── cpp_module_05
    │   ├── ex00
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   └── Bureaucrat.hpp
    │   │   └── src
    │   │       ├── Bureaucrat.cpp
    │   │       └── main.cpp
    │   ├── ex01
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   ├── Bureaucrat.hpp
    │   │   │   └── Form.hpp
    │   │   └── src
    │   │       ├── Bureaucrat.cpp
    │   │       ├── Form.cpp
    │   │       └── main.cpp
    │   ├── ex02
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   ├── AForm.hpp
    │   │   │   ├── Bureaucrat.hpp
    │   │   │   ├── PresidentialPardonForm.hpp
    │   │   │   ├── RobotomyRequestForm.hpp
    │   │   │   └── ShrubberyCreationForm.hpp
    │   │   └── src
    │   │       ├── AForm.cpp
    │   │       ├── Bureaucrat.cpp
    │   │       ├── main.cpp
    │   │       ├── PresidentialPardonForm.cpp
    │   │       ├── RobotomyRequestForm.cpp
    │   │       └── ShrubberyCreationForm.cpp
    │   ├── ex03
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   ├── AForm.hpp
    │   │   │   ├── Bureaucrat.hpp
    │   │   │   ├── Intern.hpp
    │   │   │   ├── PresidentialPardonForm.hpp
    │   │   │   ├── RobotomyRequestForm.hpp
    │   │   │   └── ShrubberyCreationForm.hpp
    │   │   └── src
    │   │       ├── AForm.cpp
    │   │       ├── Bureaucrat.cpp
    │   │       ├── Intern.cpp
    │   │       ├── main.cpp
    │   │       ├── PresidentialPardonForm.cpp
    │   │       ├── RobotomyRequestForm.cpp
    │   │       └── ShrubberyCreationForm.cpp
    │   └── _subject
    │       └── en.subject.pdf
    ├── cpp_module_06
    │   ├── ex00
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   └── ScalarConverter.hpp
    │   │   └── src
    │   │       ├── main.cpp
    │   │       └── ScalarConverter.cpp
    │   ├── ex01
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   ├── Data.hpp
    │   │   │   └── Serializer.hpp
    │   │   └── src
    │   │       ├── main.cpp
    │   │       └── Serializer.cpp
    │   ├── ex02
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   └── Base.hpp
    │   │   └── src
    │   │       ├── Base.cpp
    │   │       └── main.cpp
    │   └── _subject
    │       └── en.subject.pdf
    ├── cpp_module_07
    │   ├── ex00
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   └── whatever.hpp
    │   │   └── src
    │   │       └── main.cpp
    │   ├── ex01
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   └── iter.hpp
    │   │   └── src
    │   │       └── main.cpp
    │   ├── ex02
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   ├── Array.hpp
    │   │   │   └── Array.tpp
    │   │   └── src
    │   │       └── main.cpp
    │   └── _subject
    │       └── en.subject.pdf
    ├── cpp_module_08
    │   ├── ex00
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   ├── easyfind.hpp
    │   │   │   └── easyfind.tpp
    │   │   └── src
    │   │       └── main.cpp
    │   ├── ex01
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   └── Span.hpp
    │   │   └── src
    │   │       ├── main.cpp
    │   │       └── Span.cpp
    │   ├── ex02
    │   │   ├── Makefile
    │   │   ├── include
    │   │   │   ├── MutantStack.hpp
    │   │   │   └── MutantStack.tpp
    │   │   └── src
    │   │       └── main.cpp
    │   └── _subject
    │       └── en.subject.pdf
    └── cpp_module_09
        ├── ex00
        │   ├── Makefile
        │   ├── include
        │   │   └── BitcoinExchange.hpp
        │   └── src
        │       ├── BitcoinExchange.cpp
        │       └── main.cpp
        ├── ex01
        │   ├── Makefile
        │   ├── include
        │   │   └── RPN.hpp
        │   └── src
        │       ├── main.cpp
        │       └── RPN.cpp
        ├── ex02
        │   ├── Makefile
        │   ├── include
        │   │   └── PmergeMe.hpp
        │   └── src
        │       ├── main.cpp
        │       └── PmergeMe.cpp
        └── _subject
            └── en.subject.pdf
```
</details>

## 📌 - Key Topics

### Object-Oriented Programming (OOP)

Object-Oriented Programming (OOP) is a programming paradigm based on the concept of objects, which can contain data, in the form of fields (also known as attributes or properties), and code, in the form of procedures (often known as methods). 

OOP emphasizes the design of software through the creation and interaction of objects, aiming to make code more modular, reusable, and easier to maintain. 

It is structured around four key principles: encapsulation, inheritance, polymorphism, and abstraction. 

These principles define how data is organized, how objects interact, and how the complexity of systems is managed.

- __Encapsulation__: Understanding the bundling of data and functions that operate on that data within classes and objects.
- __Inheritance__: Learning how classes can inherit attributes and methods from other classes, enabling code reuse and extensibility.
- __Polymorphism__: Mastering how objects of different classes can be treated as objects of a common superclass, allowing for flexibility in method implementation.
- __Abstraction__: Grasping how to expose essential features while hiding implementation details to simplify interaction with objects.

### C++

C++ is a high-level programming language developed by Bjarne Stroustrup in 1985 as an extension of C, incorporating object-oriented programming (OOP) principles. 

It supports multiple paradigms, including procedural, object-oriented, and generic programming, making it highly versatile.

C++ is widely used for applications like operating systems, game engines, and real-time systems due to its flexibility and performance.

Key Features:
- Object-Oriented Programming (OOP): Facilitates encapsulation, inheritance, polymorphism, and abstraction, allowing modular and reusable code.
- Memory Management: Offers low-level control with manual memory allocation, giving developers fine control over resources.
- Templates: Enables generic programming, creating reusable code for different data types.
- Standard Template Library (STL): Provides efficient data structures and algorithms, improving development speed and reliability.
- Performance: Known for its efficiency, balancing high performance with complex abstractions, making it suitable for system-level programming and resource-intensive applications.

## 🛠️ - Usage

```sh
git clone https://github.com/kichkiro/CPP_Modules.git
cd CPP_Modules/project/
```

Now it is possible to access the various cpp_module_0[0-9] modules, each of which can be compiled with the Makefile inside them.

## ⚖️ - License

See [LICENSE](LICENSE)