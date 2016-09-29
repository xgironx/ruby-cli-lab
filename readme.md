# Ruby CLI Lab

Today is _your_ chance to practice Ruby. You'll have the option to choose one of
three prompts:

- [Battleship](./battleship.md)
- [Flash Cards](./flash_cards.md)
- [Personal Finance](./personal_finance.md)

## Getting Started

Think about how you want to structure your application. Will you have a `Menu` class?

Here's an example:

```rb
class Menu
  def self.display
    while 1
      puts "Choose one of the following:"
      puts "1 - Option 1"
      puts "2 - Option 2"
      puts "3 - Option 3"
      input = gets.chomp
      if ["1","2","3"].include? input
        self.select input
        break
      else
        puts "Invalid option."
      end
    end
  end
  def self.select number
    puts "You selected #{number}"
  end
end

Menu.display
```

What other classes will you have?
