# livepeerar.js

> This SDK/package is your go-to solution for enhancing the Livepeer Broadcast components with virtual filters and augmented reality such as Virtual backgrounds, AR filters, Faceless streaming etc.Whether you're a developer looking to build Tiktok/snapchat clones or build out Virtual-try-on products on the Livepeer infrastruture, this code sample and SDK will help you achieve these in a short time.

[![NPM](https://img.shields.io/npm/v/livepeerjs-player-filters.svg)](https://www.npmjs.com/package/livepeerjs-ar) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

## Install

```bash
npm install --save livepeerjs-ar
```

## Usage

```jsx
    import {BroadcastAR} from 'livepeerjs-player-filters'
    import * as Broadcast from "@livepeer/react/broadcast";
    import { getIngest } from "@livepeer/react/external";

    ....
    <BroadcastAR
         videoRef={videoRef}
         isSelect={isSelect}
         setisSelected={setisSelected}
         opt={opt}
         className="w-1/2 h-full"
       >
         <Broadcast.Root ingestUrl={getIngest("1606-8tzu-37cl-1wsj")}>
               <Broadcast.Container className='w-full'>
                 
                      <Broadcast.Video
                          title="Livestream"
                          style={{ height: "100%", width: "100%" }}
                          className={isSelect?.length>0?"hidden":"relative "}
                          ref={videoRef} 
                          
                          
                      />
                  </Broadcast.Container>
             </Broadcast.Root>
        
    </BroadcastAR>
```

## License

MIT © [livepeerAiSuites](https://github.com/livepeerAiSuites)
