# SQUABIX State Machine

A small state machine. States are child nodes. A machine is also a state, so you can nest them.

## Classes

- `State`
- `StateMachine`
- `MirrorStateMachine`

## Use

1. Add a `StateMachine` node.
2. Add `State` nodes under it.
3. Set `initial_state` on the machine.
4. Extend `State` to write your own states.
5. Override `enter()`, `exit()`, `update()`, `physics_update()`, and `handle_input()`.
6. Call `transition_to()` to change state.

A state cannot be replaced by a state with lower `priority`.
`MirrorStateMachine` copies the state of another machine.

## Demo

See it in the game: https://github.com/squabix/craftlander

## Needs

Godot 4.5 or newer.

## License

MIT. See `LICENSE`.
Icons are from another project. See `THIRD_PARTY.md`.
