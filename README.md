Will work in your browser after the first compilation.
Web runner now wont be unable to resolve.
Everything is fixed and minimized.


Example usage in react project:

import { solidityCompiler } from "../../browser-solidity-compiler/src/index";


  const compile = async() =>{
    const version = 'soljson-v0.8.20+commit.a1b79de6.js'; 
    const result = await solidityCompiler({
      version: `https://binaries.soliditylang.org/bin/${version}`,
      contractBody: contractCode,
      options:{optimizer:{enabled:true,runs:1000}}
    })
    return result;
  }




