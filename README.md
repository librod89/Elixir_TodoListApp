# Elixir_TodoListApp
A todo list application with a server supervisor and cache written in Elixir

Code help from https://github.com/learnelixirtv/todo

![alt tag](https://github.com/librod89/Elixir_TodoListApp/blob/master/rsz_screenshot_from_2016-12-28_13-07-35.png)

# Next Steps

Currently, when a TodoList is killed, the cache saves that state so the todos in the killed process are saved and reinstated. But if the server is killed, no todo lists are remembered. Upgrade the code so you can safely kill the Todo.Server without losing any Todo.Lists or any of their items.

## Installation

  1. Add todo to your list of dependencies in mix.exs:

        def deps do
          [{:todo, "~> 0.0.1"}]
        end

  2. Ensure todo is started before your application:

        def application do
          [applications: [:todo]]
        end
