## Protocol Buffer Message Ids

| Code | Message                     | Type
-------|-----------------------------|----------
|  1   | ServerStateMessage          | Message
| 10   | ServerWorldStateMessage     | Message
| 20   | SlugConfigureChassisRequest | Configure
| 22   | SlugConfigureCockpitRequest | Configure
| 24   | SlugConfigureTorsoRequest   | Configure
| 26   | SlugConfigureArmsRequest    | Configure
| 28   | SlugConfigureLegsRequest    | Configure
| 50   | SlugGetQueryChassisRequest  | Query
| 51   | SlugGetQueryChassisResponse | Query
| 52   | SlugGetQueryTorsoRequest    | Query
| 53   | SlugGetQueryTorsoResponse   | Query
| 54   | SlugGetQueryCockpitRequest  | Query
| 55   | SlugGetQueryCockpitResponse | Query
| 56   | SlugGetQueryArmRequest      | Query
| 57   | SlugGetQueryArmResponse     | Query
| 58   | SlugGetQueryLegRequest      | Query
| 59   | SlugGetQueryLegResponse     | Query
| 101  | ServerSlugGenericResponse   | Generic
| 102  | SlugActionLoginRequest      | Command
| 103  | SlugActionLoginResponse     | Command
| 200  | ClientActionLoginRequest    | Command
| 201  | ClientActionLoginResponse   | Command

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

From the Haskell game server:

### Configuration Error Codes

| Code | Error                       
-------|-----------------------------
| 100  | ActuatorNotFound Model
| 101  | AmmoNotFound Model
| 102  | ArmNotFound Model
| 103  | ArmNotConfigured
| 104  | ArmorNotFound Model
| 105  | CapacitorNotFound Model
| 106  | ChassisNotFound Model
| 107  | ChassisNotConfigured
| 108  | CockpitNotFound Model
| 109  | CockpitNotConfigured
| 110  | CommunicationNotFound Model
| 111  | CommunicationsOverLimit
| 112  | ComputerNotFound Model
| 113  | CounterMeasureNotFound Model
| 114  | CounterMeasureOverLimit
| 115  | EngineNotFound Model
| 116  | GyroNotFound Model
| 117  | LegNotFound Model
| 118  | LegNotConfigured
| 119  | ProtocolMismatch
| 120  | ReactorNotFound Model
| 121  | SensorNotFound Model
| 122  | SensorOverLimit
| 123  | TorsoNotFound Model
| 124  | TorsoNotConfigured
| 125  | WeaponNotFound Model
| 126  | WeaponOverLimit
