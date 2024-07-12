<div align="left"> 
  <p> 1. Library Install</p>
  <p> node, yarn, mkcert install</p>
  <pre><code>
    # 1. Install mkcert
    # windows
    choco install mkcert
    # linux
    sudo apt-get install wget libnss3-tools
    sudo apt-get install mkcert
    # mac
    brew install mkcert
  </code></pre>
  <pre><code>
    # 2. make key file
    mkcert -key-file ./key.pem -cert-file .cert.pem "localhost"
  </code></pre>
  <pre><code>
    # 3. set key "keys.pem", ".cert.pem" 
    # in "https-webrtc-screen-share/client" and "https-webrtc-screen-share/keys"
  </code></pre>
  <p> 2. To run project</p><br>
  <pre><code>
    # https-webrtc-screen-share
    # yarn or yarn install
    yarn install
    npm start
    # https-webrtc-screen-share/client
    npm start --host 0.0.0.0:3000
  </code></pre>
  <p> 3. create room and enter {your IP address}:3000/room/{your room id}</p><br>

  <p> Notice! </p>
  <p> 1. Existing rooms can be reused. </p> <br>
  <p> 2. Screen sharing is only available to the second entered host.</p>
</div>
