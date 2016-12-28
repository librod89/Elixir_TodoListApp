# Elixir_TodoListApp
A todo list application with a server supervisor and cache written in Elixir

Code help from https://github.com/learnelixirtv/todo

## Installation

  1. Add todo to your list of dependencies in mix.exs:

        def deps do
          [{:todo, "~> 0.0.1"}]
        end

  2. Ensure todo is started before your application:

        def application do
          [applications: [:todo]]
        end
