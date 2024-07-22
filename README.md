Inputs "entry" and "exit" are taken from sensors at the entry and exit doors respectively. "entry" would be high if a person is entering the room and "exit" is high if person is leaving the room.Outputs are "full", "empty", "fan", "light" and "AC".
"full" would be high when room occupancy is 3 as maximum occupancy is 3.
"empty" is high when room occupancy is zero.
Entry door gets locked when room is full and exit door gets locked when room is empty.
"fan", "light" and "AC" are turned low if room occupancy is zero, that is when "empty" is high. Else control to fan, light and AC are given to user.
As control is given to user when room is not empty, we consider actual switches of fan, light and AC also as inputs.

This is a Moore finite state machine. It consists of 4 states as maximum occupancy is 3.

S0 : empty
S1: 1 person in the room
S2 : 2 people in the room
S3 : 3 people in the room (full)

![smart_room_fsm_state_diagram](https://github.com/user-attachments/assets/be4eb830-2c19-4985-93be-6f364d0ad9d1)


