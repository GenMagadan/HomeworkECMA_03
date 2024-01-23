1. "Управление персоналом компании"

- Реализуйте класс Employee (сотрудник), который имеет следующие свойства и методы:

  - Свойство name (имя) - строка, имя сотрудника.
  - Метод displayInfo() - выводит информацию о сотруднике (имя).

- Реализуйте класс Manager (менеджер), который наследует класс Employee и имеет дополнительное свойство и метод:

  - Свойство department (отдел) - строка, отдел, в котором работает менеджер.
  - Метод displayInfo() - переопределяет метод displayInfo() родительского класса и выводит информацию о менеджере (имя и отдел).

Пример использования классов:

- const employee = new Employee(""John Smith"");
- employee.displayInfo();

Вывод: Name: John Smith

- const manager = new Manager(""Jane Doe"", ""Sales"");
- manager.displayInfo();

Вывод: Name: Jane Doe Department: Sales

2. "Управление списком заказов"

- Реализуйте класс Order (заказ), который имеет следующие свойства и методы:

  - Свойство orderNumber (номер заказа) - число, уникальный номер заказа.
  - Свойство products (продукты) - массив, содержащий список продуктов в заказе.
  - Метод addProduct(product) - принимает объект product и добавляет его в список продуктов заказа.
  - Метод getTotalPrice() - возвращает общую стоимость заказа, основанную на ценах продуктов.

Пример использования класса:

- class Product { constructor(name, price) {this.name = name; this.price = price;}}
- const order = new Order(12345);
- const product1 = new Product(""Phone"", 500);
- order.addProduct(product1);
- const product2 = new Product(""Headphones"", 100);
- order.addProduct(product2);

console.log(order.getTotalPrice());

Вывод: 600

3. Необязательное задание

Создать класс "Товар" с приватными полями "название", "цена" и "количество". Класс должен иметь публичные методы "изменить цену", "изменить количество" и "получить стоимость", которые будут изменять соответствующие поля объекта и возвращать стоимость товара соответственно. Также класс должен иметь статическое поле "максимальное количество", которое будет задавать максимально допустимое количество товара для всех создаваемых объектов.

Пример работы кода:

- const product1 = new Product('Тетрадь', 50, 200);
- console.log(product1.name); // "Тетрадь"
- console.log(product1.price); // 50
- console.log(product1.quantity); // 200
- console.log(product1.getCost()); // 10000
- const product2 = new Product('Ручка', 10, 5000); // выбросится ошибка "Quantity is too high"
