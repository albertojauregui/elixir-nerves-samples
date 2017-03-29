# Elixir Nerves

## Installation

```elixir

mix local.hex
mix local.rebar

mix archive.install https://github.com/nerves-project/archives/raw/master/nerves_bootstrap.ez
mix local.nerves
```

## Basic App

```elixir

mix new hello

```

## Blinky RPi

```elixir

mix nerves.new rpi_blink
cd rpi_blink
MIX_TARGET=rpi3 mix deps.get
MIX_TARGET=rpi3 mix firmware
MIX_TARGET=rpi3 mix firmware.burn
```

## Blinky

```elixir

mix nerves.new blinky
cd blinky
MIX_TARGET=rpi3 mix deps.get
MIX_TARGET=rpi3 mix firmware
MIX_TARGET=rpi3 mix firmware.burn

```