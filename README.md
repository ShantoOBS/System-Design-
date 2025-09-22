<h2>System Design (Short Notes)</h2>

<h3>Definition</h3>
<p>
  System design is the process of defining the architecture and components of a software system 
  to meet business requirements like scalability, maintainability, performance, and security.
</p>

<h3>System Design in SDLC</h3>
<ul>
  <li>Essential step before implementation/testing.</li>
  <li>Provides business logic backbone and handles exceptional scenarios.</li>
</ul>

<h3>Types of Design</h3>
<h4>1. High-Level Design (HLD)</h4>
<ul>
  <li>Big picture: architecture, major components, data flow, technology stack.</li>
  <li>Done by architects/managers.</li>
  <li><b>Example:</b> Netflix migrated from monolith to microservices.</li>
</ul>

<h4>2. Low-Level Design (LLD)</h4>
<ul>
  <li>Detailed blueprint for developers.</li>
  <li>Covers class diagrams, DB schemas, APIs, error handling, design patterns.</li>
  <li><b>Example:</b> defining tables, methods, request/response formats.</li>
</ul>

<h3>Steps in System Design</h3>
<ol>
  <li>Understand requirements.</li>
  <li>Define system architecture.</li>
  <li>Choose technology stack.</li>
  <li>Design modules.</li>
  <li>Plan for scalability.</li>
  <li>Ensure security & privacy.</li>
  <li>Test & validate design.</li>
</ol>

<h3>Interview Approach</h3>
<ul>
  <li>Break problem into components/features.</li>
  <li>Communicate ideas clearly (whiteboard, diagrams).</li>
  <li>Make reasonable assumptions (traffic, DB calls, caching).</li>
</ul>

<h3>Key Considerations</h3>
<ul>
  <li><b>Scalability</b> – handle growth.</li>
  <li><b>Performance</b> – fast & efficient.</li>
  <li><b>Reliability</b> – minimal downtime.</li>
  <li><b>Security</b> – protect data.</li>
  <li><b>Maintainability</b> – easy to update.</li>
  <li><b>Interoperability</b> – integrate with other systems.</li>
  <li><b>Usability</b> – user-friendly.</li>
  <li><b>Cost-effectiveness</b> – efficient resource use.</li>
</ul>

<hr/>

<h2>Requirements Analysis</h2>
<p>
  Requirements analysis is an essential step in software development. It ensures that a system meets business objectives and user needs.
  Requirements are usually divided into <b>Functional</b> and <b>Non-Functional</b>.
</p>

<h3>Functional Requirements (FRs)</h3>
<p>
  Define <b>what the system should do</b> — specific features, tasks, or operations.
</p>
<ul>
  <li>User authentication, data entry, search functionality, payment handling, report generation.</li>
  <li><b>Example Questions:</b> What features should be designed? What edge cases must be considered?</li>
</ul>

<h3>Non-Functional Requirements (NFRs)</h3>
<p>
  Define <b>how the system should perform</b> — quality attributes like speed, scalability, or security.
</p>
<ul>
  <li>Performance, Security, Usability, Reliability, Scalability, Maintainability, Portability.</li>
  <li><b>Example Questions:</b> How fast should the system respond? How secure should it be?</li>
</ul>

<h3>Extended Requirements</h3>
<p>
  Cover business goals, domain-specific needs, or long-term considerations 
  (e.g., compliance, cost, market adaptation).
</p>

<h3>Examples</h3>
<h4>1. Online Banking System</h4>
<ul>
  <li><b>FRs:</b> Login, check balance, transaction notifications.</li>
  <li><b>NFRs:</b> Respond in &lt;2s, encrypted transactions, handle 100M users.</li>
</ul>
<h4>2. Food Delivery App</h4>
<ul>
  <li><b>FRs:</b> Browse menu, place orders, track orders, make payments.</li>
  <li><b>NFRs:</b> Load menu &lt;1s, support 50K concurrent orders, intuitive interface.</li>
</ul>

<h3>Differences Between FRs and NFRs</h3>
<ul>
  <li><b>Definition:</b> FRs = What system does, NFRs = How system works.</li>
  <li><b>Purpose:</b> FRs = Features/behavior, NFRs = Quality/experience.</li>
  <li><b>Measurement:</b> FRs = outputs/results, NFRs = benchmarks/metrics.</li>
  <li><b>Impact:</b> FRs drive design/features, NFRs shape architecture/performance.</li>
</ul>

<h3>Why Balance Both?</h3>
<ul>
  <li>Improves User Experience.</li>
  <li>Enhances performance & reliability.</li>
  <li>Prevents failures & bottlenecks.</li>
  <li>Reduces long-term costs.</li>
  <li>Supports future system evolution.</li>
</ul>

<h3>Challenges in Defining Requirements</h3>
<ul>
  <li>Ambiguity or incomplete requirements.</li>
  <li>Changing needs over time.</li>
  <li>Difficulty prioritizing functional vs. non-functional.</li>
  <li>Hard to measure NFRs.</li>
  <li>Conflicting trade-offs (e.g., security vs. performance).</li>
</ul>

<h3>Gathering Requirements</h3>
<ul>
  <li><b>Functional:</b> Interviews, surveys, workshops.</li>
  <li><b>Non-Functional:</b> Performance benchmarks, security standards, usability testing.</li>
</ul>

<hr/>

<h1>Object-Oriented Programming (OOP)</h1>

<p>
  Object-Oriented Programming (OOP) is a paradigm that helps you write modular, reusable, 
  and scalable code by organizing it around <b>classes</b> (blueprints) and 
  <b>objects</b> (instances of those blueprints).
</p>

<p>
  In simple terms, OOP is about designing a system as a collection of objects, 
  each with its own <b>data (state)</b> and <b>methods (behaviors)</b> 
  that interact to solve problems.
</p>

<hr/>

<h2>Why OOP is Needed</h2>
<ul>
  <li>Changes in one team's code may break others → difficult to maintain.</li>
  <li>Large number of parameters during function calls.</li>
  <li>Difficult to divide and maintain code across teams.</li>
  <li>Limited code reusability.</li>
  <li>Not scalable as the code is not modular.</li>
</ul>

<hr/>

<h2>Real-world Examples</h2>
<ul>
  <li>Banking System</li>
  <li>E-commerce Platform</li>
  <li>Hospital Management System</li>
</ul>

<hr/>

<h2>Classes and Objects</h2>

<h3>1. Classes</h3>
<p>
  A <b>class</b> is a blueprint that defines the <i>attributes</i> (data) 
  and <i>methods</i> (functions). Example: Car class → attributes (make, model, year), 
  methods (startEngine, accelerate).
</p>

<h3>2. Objects</h3>
<p>
  An <b>object</b> is an instance of a class with its own values.
</p>

<pre>
<code>
#include &lt;iostream&gt;
using namespace std;

class Student {
public:
    int roll;
    string name;

    void takeLeave() {
        cout &lt;&lt; "on leave" &lt;&lt; endl;
    }

    void bunkClass() {
        cout &lt;&lt; "Go out and play" &lt;&lt; endl;
    }
};

int main() {
    Student sid;
    sid.bunkClass();
    sid.name = "Siddhartha Hazra";
    cout &lt;&lt; sid.name &lt;&lt; endl;
    return 0;
}
</code>
</pre>

<hr/>

<h2>Encapsulation</h2>
<p>
  Encapsulation means <b>wrapping data and methods into a single unit (class)</b>. 
  It hides implementation details and exposes only necessary parts.
</p>
<ul>
  <li><b>Private</b> → accessible only inside the class</li>
  <li><b>Public</b> → accessible from outside</li>
  <li><b>Protected</b> → accessible in subclasses</li>
</ul>

<pre>
<code>
#include &lt;iostream&gt;
#include &lt;string&gt;
using namespace std;

class Employee {
private:
    int id;
    string name;

public:
    void setId(int id) { this-&gt;id = id; }
    void setName(string name) { this-&gt;name = name; }

    int getId() { return id; }
    string getName() { return name; }
};

int main() {
    Employee emp;
    emp.setId(101);
    emp.setName("Geek");

    cout &lt;&lt; "Employee ID: " &lt;&lt; emp.getId() &lt;&lt; endl;
    cout &lt;&lt; "Employee Name: " &lt;&lt; emp.getName() &lt;&lt; endl;

    return 0;
}
</code>
</pre>

<hr/>

<h2>Abstraction</h2>
<p>
  Abstraction focuses on <b>essential features</b> while hiding unnecessary details.
</p>
<ul>
  <li><b>Abstract Class</b> → provides a blueprint with some implemented methods.</li>
  <li><b>Interface</b> → defines method signatures only.</li>
</ul>

<pre>
<code>
#include &lt;iostream&gt;
using namespace std;

class Vehicle {
public:
    virtual void accelerate() = 0;
    virtual void brake() = 0;

    void startEngine() {
        cout &lt;&lt; "Engine started!" &lt;&lt; endl;
    }
};

class Car : public Vehicle {
public:
    void accelerate() override {
        cout &lt;&lt; "Car accelerating..." &lt;&lt; endl;
    }
    void brake() override {
        cout &lt;&lt; "Car braking..." &lt;&lt; endl;
    }
};

int main() {
    Vehicle* myCar = new Car();
    myCar-&gt;startEngine();
    myCar-&gt;accelerate();
    myCar-&gt;brake();
    delete myCar;
    return 0;
}
</code>
</pre>

<hr/>

<h2>Inheritance</h2>
<p>
  Inheritance allows a <b>child class</b> to use properties/methods of a <b>parent class</b>.
</p>

<pre>
<code>
#include &lt;iostream&gt;
using namespace std;

class Animal {
public:
    void eat() { cout &lt;&lt; "Animal eating" &lt;&lt; endl; }
    void sleep() { cout &lt;&lt; "Animal sleeping" &lt;&lt; endl; }
};

class Dog : public Animal {
public:
    void bark() { cout &lt;&lt; "Dog barking!" &lt;&lt; endl; }
};

int main() {
    Dog myDog;
    myDog.eat();
    myDog.sleep();
    myDog.bark();
    return 0;
}
</code>
</pre>

<hr/>

<h2>Polymorphism</h2>
<p>
  Polymorphism means "many forms". It allows methods to behave differently 
  depending on the object type.
</p>
<ul>
  <li><b>Method Overriding</b> → subclass redefines a method from parent.</li>
  <li><b>Method Overloading</b> → same method name with different parameters.</li>
</ul>

<pre>
<code>
#include &lt;iostream&gt;
using namespace std;

class Calculator {
public:
    int add(int a, int b) { return a + b; }
    int add(int a, int b, int c) { return a + b + c; }
    double add(double a, double b) { return a + b; }
};

int main() {
    Calculator calc;
    cout &lt;&lt; calc.add(5, 3) &lt;&lt; endl;
    cout &lt;&lt; calc.add(4, 6, 2) &lt;&lt; endl;
    cout &lt;&lt; calc.add(3.5, 2.7) &lt;&lt; endl;
    return 0;
}
</code>
</pre>

<hr/>

<h2>SOLID Principles</h2>

<h3>1. Single Responsibility Principle (SRP)</h3>
<p>
  A class should have only one reason to change.  
  Each class should handle only one job or responsibility.
</p>
<p><b>Example:</b> A <i>InvoicePrinter</i> class only prints invoices,  
while <i>InvoiceCalculator</i> only calculates totals.</p>

<h3>2. Open/Closed Principle (OCP)</h3>
<p>
  Software entities should be <b>open for extension</b> but <b>closed for modification</b>.  
  Add new features by extending the code, not by changing existing code.
</p>
<p><b>Example:</b> Instead of editing a payment class to add PayPal,  
you create a new <i>PayPalPayment</i> class that extends the <i>Payment</i> interface.</p>

<h3>3. Liskov Substitution Principle (LSP)</h3>
<p>
  Objects of a child class should be replaceable with objects of the parent class  
  without breaking the program.  
  Child classes must honor the "rules" defined by the parent.
</p>
<p><b>Example:</b> A <i>Sparrow</i> (child) can replace a <i>Bird</i> (parent)  
and still respect the parent’s behavior like "fly()".  
Child class may extend behavior but must not break parent rules.</p>

<h3>4. Interface Segregation Principle (ISP)</h3>
<p>
  Clients should not be forced to depend on methods they do not use.  
  Instead of one large interface, use many small, specific interfaces.
</p>
<p><b>Example:</b> A <i>Printer</i> interface with only "print()" is better than  
a big "Machine" interface that forces classes to also implement "scan()" or "fax()" unnecessarily.</p>

<h3>5. Dependency Inversion Principle (DIP)</h3>
<p>
  High-level modules should not depend on low-level modules.  
  Both should depend on abstractions (interfaces or abstract classes).
</p>
<p><b>Example:</b> A <i>Chef</i> (high-level) depends on an <i>Oven interface</i>,  
not on a specific brand like Samsung or LG.  
This way, any oven can be swapped without changing the chef’s code.</p>

<hr/>
<h1>Software Development Principles</h1>

<h2>DRY Principle</h2>
<p>
  <b>DRY</b> stands for <i>Don't Repeat Yourself</i>. Avoid duplicating code or logic. 
  Instead, reuse functions, modules, or classes to make the code easier to maintain.
</p>

<h2>KISS Principle</h2>
<p>
  <b>KISS</b> stands for <i>Keep It Simple, Stupid</i>. Design software in the simplest way possible, 
  avoiding unnecessary complexity. Simple code is easier to read, test, and maintain.
</p>

<h2>YAGNI Principle</h2>
<p>
  <b>YAGNI</b> stands for <i>You Aren't Gonna Need It</i>. Only implement features that are currently required. 
  Avoid adding functionality for future use unless necessary.
</p>

<h2>Comments in Code</h2>
<p>
  Use comments to explain <b>why</b> the code does something, not <b>what</b> it does. 
  Good comments improve readability and maintainability.
</p>

<h2>GRASP Principles in OOAD</h2>
<p>
  <b>GRASP</b> (General Responsibility Assignment Software Patterns) are guidelines for assigning responsibilities in Object-Oriented Analysis and Design:
</p>
<ul>
  <li><b>Controller</b> – Handles system events and delegates work.</li>
  <li><b>Creator</b> – Responsible for creating instances of related classes.</li>
  <li><b>Information Expert</b> – Assign responsibilities to the class with the necessary information.</li>
  <li><b>Low Coupling</b> – Reduce dependencies between classes.</li>
  <li><b>High Cohesion</b> – Keep related responsibilities together.</li>
  <li><b>Polymorphism</b> – Use polymorphic behavior to handle variations.</li>
  <li><b>Pure Fabrication</b> – Create classes that do not represent domain concepts to achieve better design.</li>
  <li><b>Indirection</b> – Use intermediary objects to reduce direct coupling.</li>
  <li><b>Protected Variations</b> – Protect elements from changes in other elements by encapsulating variations.</li>
</ul>

