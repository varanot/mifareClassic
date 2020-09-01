# javax.smartcardio
The specificiation describes the Java Smart Card I/O API defined by JSR 268. It defines a Java API for communication with Smart Cards using ISO/IEC 7816-4 APDUs. It thereby allows Java applications to interact with applications running on the Smart Card, to store and retrieve data on the card, etc.

The API is defined by classes in the package javax.smartcardio. They can be classified as follows:
* Classes describing the corresponding Smart Card structures: ATR, CommandAPDU, ResponseAPDU 
* Factory to obtain implementations: TerminalFactory 
* Main classes for card and terminal functions: CardTerminals, CardTerminal, Card, CardChannel 
* Supporting permission and exception classes: CardPermission, CardException, CardNotPresentException 
* Service provider interface, not accessed directly by applications: TerminalFactorySpi

|      CLASS       |                          DESCRIPTION                              |
|:-----------------|:------------------------------------------------------------------|
|ATR               |A SmartCard's answer to reset Bytes                                |
|Card              |A SmartCard with which a connection has been established           |
|CardChannel       |A logical channel connection to a SmartCard                        |
|CardPermission    |A permission for SmartCard operations                              |
|CardTerminal      |A SmartCard terminal, sometimes referred to as a SmartCard Reader  |
|CardTerminals     |The set of terminals supported by a TerminalFactory                |
|CommandAPDU       |A command APDU following the structure of ISO/IEC 7816-4           |
|ResponseAPDU      |A response APDU as defined in ISO/IEC 7816-4                       |
|TerminalFactory   |A factory for CardTerminal objects                                 |
|TerminalFactorySpi|The TerminalFactorySpi class defines the service provider interface|
