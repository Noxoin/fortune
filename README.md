# Fortune - Financial tracker

Fortune is a financial tracker that stores your transaction information based on accounts.

## Background

I wanted a simple way to keep track of all the transactions that occur during my day to day. My first 
iteration on solving this was via excel in 2014. It worked fine until I had to deal with multiple 
currencies and didn't know how to adapt to it. Also, the metrics gathered weren't queried and I was 
very tied down to making everything on a monthly basis for tracking. I ported my excel sheet to 
[Google sheets](https://go.noxoin.com/financial-tracker-demo) due to its ability to sync across devices.

Now, I want to be able to do more with my transaction data, and possibly query out new information in 
a more intuitive mannor.

You can view a live version of this code @ [fortune.noxoin.com](https://fortune.noxoin.com/).

## Development

### Datastore Emulation

During development and testing, you will need to have an emulated datastore by 
following instructions [here](https://cloud.google.com/appengine/docs/standard/go/tools/using-local-server).

```
# Start emulated datastore for dev environment
gcloud beta emulators datastore start
```

Also, remember to set your environment variable on each terminal that runs the 
application.

```
# Have application pointing to dev environment and not prod datastore
$(gcloud beta emulators datastore env-init)
```

Run the start.sh script to start the server.

## License

	The code in this repository is licensed under the Apache License, Version 2.0 (the "License");
	you may not use this file except in compliance with the License.
	You may obtain a copy of the License at

		http://www.apache.org/licenses/LICENSE-2.0

	Unless required by applicable law or agreed to in writing, software
	distributed under the License is distributed on an "AS IS" BASIS,
	WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
	See the License for the specific language governing permissions and
	limitations under the License.

**NOTE**: This software depends on other packages that may be licensed under different open source licenses.
