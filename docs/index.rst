.. Copyright (c) 2015 Pietro Albini <pietro@pietroalbini.io>
   Released under the MIT licende

~~~~~~~~~~~~~~~~~~~~~~
botogram documentation
~~~~~~~~~~~~~~~~~~~~~~

*A microframework for Telegram bots.*

botogram is a MIT-licensed microframework, which aims to simplify the creation
of `Telegram bots`_. It offers a concise, simple API, which allows you to spend
all your creativity in the bot, without worrying about anything else.

It also provides a robust, fully scalable bot runner process, which will be
able to process fastly high workloads. And as if this isn't enough, it has
builtin support for commands, with an automatically-generated ``/help``
command.

::

   import botogram
   bot = botogram.create("YOUR-API-KEY")

   @bot.command("hello")
   def hello_command(chat, message, args):
      """Say hello to the world!"""
      chat.send("Hello world")

   bot.run()

.. toctree::
   :maxdepth: 2

.. _Telegram bots: https://core.telegram.org/bots
