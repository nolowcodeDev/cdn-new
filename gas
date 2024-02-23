    const runScript = async function(functionName, data={}) {
      return new Promise((resolve, reject) => {
        google.script.run.withSuccessHandler((result) => {
          resolve(JSON.parse(result))
        }).withFailureHandler((error) => {
          reject(error)
        })[functionName](JSON.stringify(data))
      })
    }
