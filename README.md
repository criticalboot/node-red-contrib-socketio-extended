# node-red-contrib-socketio-extended
Implementation for [Node-RED](https://nodered.org/) of the popular [Socket.IO](http://socket.io/).

It is forked from `node-red-contrib-socketio` since the original package seems not to be maintained anymore.
Therefor some pending pull requests from the original repo are already implemented in this one.
* CORS support

## Installation
To install node-red-contrib-socketio use this command

`npm i node-red-contrib-socketio-extended`

## Composition
The Socket.IO implementation is made with
* 1 configuration Node that holds the server definitions and the user can decide to bind the SocketIO server on the Node-RED port or bind it to another port
* 1 input node where the user adds all the `topic`s in which they are interested
* 1 output node that sends the data received into `msg.payload`
* 1 node to join a Socket IO room
* 1 node to leave a Socket IO room

## Usage
To see an example usage go to [Example Chat App](https://flows.nodered.org/flow/71f7da3a14951acb67f94bac1f71812a)

## License
MIT

## Thanks
Thank to: 
* @nexflo for translating the comments in English and for pre-sending control data 
* @bimalyn-IBM for implementing rooms
* @essuraj for implementing rooms listing node
* @cazellap for adding compatibility to socketIO 3.0
* @
