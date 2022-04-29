# I can make anything

## I can program fluently

### Personal Thoughts: What does it mean to be able to program fluently?

I believe that being able to program fluently is not about knowing language off the top of your head, an important part is being able to visualise and use diagramming to layout how you plan to write the code to solve the challenge. One of the skills I have learnt during my time on Makers is that I have more confidence in being able to research concepts that I might not be familiar with in a language. For example, I know that Ruby has functionality to achieve X so I can research how that might be achieved in Javascript. 

One of the tasks we were set was to create a list of the differences between Ruby and Javascript.

```
JS vs Ruby Syntax 
===============
Classes (class Frame)

	JAVASCRIPT: Class
	================

class Hello {
constructor(name) { 			// constructor is like initialize in ruby
this.name = name;		// this. like @name in ruby
};

		sayName() {
			return `Hello ${this.name}`
		};
	};

	RUBY: Class
	==========

	class Hello 
		def initialize(name)
			@name = name
		end
	
		def sayName
			puts “Hello #{name}
		end
	
	end
	

Private: in classes

	JAVASCRIPT: Private functions
	========================

_methodName 		// treat it as if it’s private

#privateMethodName 		// is private and only accessible inside a class

RUBY: Private methods
==================

	private 		# written above the methods within the class

Variables (a = 5)

	JAVASCRIPT: let
	=============

	let name = “Claire”; 		// mutable

	RUBY: variable
	===========
	
	name = “Claire”

Constants (CONSTANT = 5)

	JAVASCRIPT: const
	===============
	
	const NAME = “Claire”;		// convention states to use uppercase 

	RUBY: const
	==========
	
	NAME = “Claire” 		# convention states to use uppercase

Addition ( 6 + 4 )

	JAVASCRIPT & RUBY: Same
	=======================

Methods (def some_method)

JAVASCRIPT: Arrow Function
=======================

	let sayHello = (name) => {
		return `Hello ${name}`;
	}
	sayHello(‘Claire’);

	OR: one line syntax
	===============

	let sayHello = name => `Hello ${name}`;	 // note the use of backticks!
	console.log(sayHello(“Claire”); 	// need to use console.log as there is no return

	UNLESS
The function is inside a class:

	sayHello () {
		`Hello ${this.name}`; 		// with this.name set in the constructor
	}

	RUBY: Methods
	============

	def say_hello (name)
		Puts “Hello #{name}”		# note the use of double quotation marks!
	end
	puts say_hello(“Claire”)		# need to use ‘puts’ or ‘print’ 

If else (if x then some_method end)

	JAVASCRIPT: If, else if, else
	======================
	if (num === 0) {		// note the ‘===’ for strict equality 
		return “Hello”; 
	} else if (num > 10) {
		return “Bye”;
	} else { 
	return “Hello, bye”;
	}
	
	RUBY: if, elsif, end
	==============

	if num == 0 		# note the ‘==’ for strict equality
		puts “Hello”
	elsif num > 10
		puts “Bye”
	else	
		puts “Hello, bye”
	end

	
Arrays (my_array = []) (my_array.push etc.)
	
Loops (while, loop do, 5.times etc.)

	JAVASCRIPT: For
	==============

	for (let i = 0; i < 10; i++) {
		return i;
	}
	
	RUBY: For
	========
	
	for num in 1..10 do
		puts num
	end

	OR

	[1, 3, 9].each { |num| puts num }
	
	OR		# can use curly braces or do/end
	
	[1, 3, 9].each do |num| 
puts num
end

—----------------

JAVASCRIPT: While
===============



RUBY: While loop
==============

num = 10
while num < 20 
	puts num
	num += 1
end
	
Instance, Class variables (@instance_variable, @@class_variable)
	
IO, (gets, chomp, puts, print, p etc)
Testing (rspec)

	JAVASCRIPT: Jest
	==============

	npm install jest	// installs jest and creates the node_modules folder
	.gitignore		// inside write: node_modules to exclude from .git
	
	touch hello.test.js 		// jest test file is test.js

	describe(‘Hello’, () => {	
		it(‘what the test does’, () => {		// uses the same arrow function syntax
		// write out what you want to test
		// eg. expect(.....).toBe(.....);
		});
	});

	const Hello = require(‘./hello’); 	// inside the test file to require the .js file
	module.exports = Hello;		// at the bottom of the .js file to export the file

	RUBY: rspec
	==========

	rspec –init 	# initializes your directory for rspec and creates the spec folder/helper
	rspec 		# runs rspec testing on your file

	require 
	
	
	
Data types (strings, numbers, booleans etc.)
TDD/rspec
Everything is an object in ruby.
Hashes (my_hash = Hash.new, my_hash = {:key => ‘value

	JAVASCRIPT: Object
	=================

	const aboutMe = {
		name: “Claire,
		location: “London”
	};

	RUBY: Hash
	==========

	about_me = {
		name: “Claire”,
		location: “London”
	}
	
Mathematical operators ( +, - , *, /)

	JAVASCRIPT & RUBY: Same
	=======================

Procs, blocks, lambdas (do..end, Proc.new)
Gems/bundler

	JAVASCRIPT: Npm/Package.json
	==========================
	
	npm init -y 		// creates the package.json files and lock

	RUBY: Bundle/Gemfile
	=================
	
	bundle init 		# creates a Gemfile
	gem list		# shows all installed gems
	
	

Inheritance
Polymorphism
Struct
irb
	
	JAVASCRIPT: Node.js
	=================
	
	>> node		// opens the node REPL in the command line
	>> node file.js		// opens that specific file in the node REPL

	RUBY: irb or ruby
	=============
	
	>> irb			# opens the irb REPL in the command line
	>> irb -r “./file.rb”		# opens that specific file in the irb REPL
 	>> ruby file.rb		# opens that specific file in the ruby REPL
	
Comparators (==, <=, > etc.)

	JAVASCRIPT: Strict equality operator
	============================
	
	num === 0 		// three ‘=’ signs

	RUBY: Strict equality operator
	=======================

	num == 0		# two ‘=’ signs

	
Ternary (x > 5 ? do_something : do_something_else)
Built in methods
Time
Random
Errors - (raise)
Comments (# Look here)

	JAVASCRIPT: Comments
	===================

	// single line comment

	/* multi
	    line comment */

	RUBY: Comments
	==============

	# single line comment

	=begin multi 
	line comment
	=end


String interpolation
	
	JAVASCRIPT: String template literals
	============================
	
	let name = “Claire”
console.log(`Hello, ${name}`)	;		// note the use of backticks and $

OR

return `Hello, ${name}`;	

RUBY: String interpolation
====================

name = “Claire”
puts “Hello #{name}”

OR

name = “Claire”
print “Hello #{name}”
```


