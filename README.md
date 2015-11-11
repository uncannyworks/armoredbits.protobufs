## Protocol Buffer Message Ids

| Code | Message                       | Type
-------|-------------------------------|----------
|  1   | ServerStateMessage            | Message
| 10   | ServerWorldStateMessage       | Message
| 20   | SlugConfigureChassisRequest   | Configure
| 22   | SlugConfigureCockpitRequest   | Configure
| 24   | SlugConfigureTorsoRequest     | Configure
| 26   | SlugConfigureArmsRequest      | Configure
| 28   | SlugConfigureLegsRequest      | Configure
| 30   | SlugConfigureDoneRequest      | Configure
| 50   | SlugGetQueryWarMachineRequest | Query
| 51   | SlugGetQueryWarMachineReponse | Query
| 101  | ServerSlugGenericResponse     | Generic
| 102  | SlugActionLoginRequest        | Command
| 103  | SlugActionLoginResponse       | Command
| 200  | ClientActionLoginRequest      | Command
| 201  | ClientActionLoginResponse     | Command

## Server State Codes

| Code | State
-------|-----------------------------
| 1    | Initializing
| 2    | WaitingForSlugs
| 3    | Ready

## World State Codes

| Code | State
-------|-----------------------------
| 1    | Initializing
| 2    | ConfigurationPhase
| 3    | StartupPhase
| 4    | GamePhase
| 5    | GameOverPhase

## Error Codes

### State Error Codes

| Code | Error                       
-------|-----------
| 50   | WrongState

### Configuration Error Codes

| Code | Error                       
-------|-----------------------------
| 100  | ActuatorNotFound Model
| 101  | AmmoNotFound Model
| 102  | ArmNotFound Model
| 103  | ArmNoIndex ComponentId
| 104  | ArmNotConfigured
| 105  | ArmorNotFound Model
| 106  | CapacitorNotFound Model
| 107  | ChassisNotFound Model
| 108  | ChassisNotConfigured
| 109  | CockpitNotFound Model
| 110  | CockpitNotConfigured
| 111  | CommunicationNotFound Model
| 112  | CommunicationsOverLimit
| 113  | ComputerNotFound Model
| 114  | CounterMeasureNotFound Model
| 115  | CounterMeasureOverLimit
| 116  | EngineNotFound Model
| 117  | GyroNotFound Model
| 118  | LegNotFound Model
| 119  | LegNoIndex ComponentId
| 120  | LegNotConfigured
| 121  | OverChassisMaxWeight
| 122  | ProtocolMismatch
| 123  | ReactorNotFound Model
| 124  | SensorNotFound Model
| 125  | SensorOverLimit
| 126  | TorsoNotFound Model
| 127  | TorsoNotConfigured
| 128  | WeaponNotFound Model
| 129  | WeaponOverLimit

## Simulation Codes

These are sent from the server to the 3d client.

| Code | Message
-------|---------------------------------
| 1    | ServerClientObjectSpawnMessage 
| 2    | ServerClientObjectMoveMessage 
| 3    | ServerClientObjectDestroyMessage 
