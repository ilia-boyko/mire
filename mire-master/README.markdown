# Mire

It's a nonviolent MUD. (Multi-User Dungeon)

## Usage

First make sure that you have `java` installed on your
machine. [OpenJDK](https://adoptopenjdk.net) is recommended. It should
be at least version 8, but newer versions (tested up to 17) should work too.

Do `./lein run` inside the Mire directory to launch the Mire
server. Then players can connect by telnetting to port 3333.

## Motivation

The primary purpose of this codebase is as a demonstration of how to
build a simple multithreaded server in Clojure.

Mire is built up step-by-step, where each step introduces one or two
small yet key Clojure principles and builds on the last step. The
steps each exist in separate git branches. To get the most out of
reading Mire, you should start reading in the branch called
[step-01-echo-server](http://github.com/technomancy/mire/tree/01-echo-server)
and continue from there.

While you can learn from Mire on its own, it has been written
specifically for the [PluralSight screencast on
Clojure](https://www.pluralsight.com/courses/functional-programming-clojure).
A [blog post](https://technomancy.us/136) steps through the codebase
and shows how to make minor updates for a more recent version of Clojure.

Copyright © 2009-2021 Phil Hagelberg
Licensed under the same terms as Clojure.

## Расширяемый функционал

В ходе разработки был добавлен следующий функционал:
1. команда whisper - позволяет отправить приватное сообщение игроку
2. модификация команды say - выводит имя игрока, который сказал
3. модификация команды look - выводит имена игроков, которые находятся в комнате
4. бот на prolog, который ходит по комантам и сообщает об этом

## Ход разработки

Был изменён файл commands.clj
