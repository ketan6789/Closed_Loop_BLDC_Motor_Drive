## Hall Sensor Data to Rotor Position 

This code processes the Hall sensor inputs from a BLDC motor and determines the rotor's current sector position (1 to 6). The sector information is crucial for defining the correct inverter switching logic required for proper electronic commutation.

```matlab
function sector = hall_to_sector(H_A, H_B, H_C)
% H_A, H_B, H_C are the Hall sensor inputs (0 or 1)
% sector is the output (1 to 6) indicating the rotor position

% Convert Hall sensor inputs to a unique decimal value
hall_value = H_A * 4 + H_B * 2 + H_C * 1;

switch hall_value
    case 5  % (1,0,1)
        sector = 1;
    case 4  % (1,0,0)
        sector = 2;
    case 6  % (1,1,0)
        sector = 3;
    case 2  % (0,1,0)
        sector = 4;
    case 3  % (0,1,1)
        sector = 5;
    case 1  % (0,0,1)
        sector = 6;
    otherwise
        sector = 0; % Error case (invalid Hall sensor state)
end
```
