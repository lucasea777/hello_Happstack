#Install Haskell
```
sudo apt-get install -y haskell-platform
```
#Install Happstack
```
PATH=~/.cabal/bin:$PATH cabal update
PATH=~/.cabal/bin:$PATH cabal install happstack-server
```
#Compile hello.hs
```
ghc -threaded HelloWorld.hs -o helloworld
./helloworld
```
#Run skipping compilation
```
runhaskell HelloWorld.hs
```
#Test the server:
```
curl http://localhost:8000
```

