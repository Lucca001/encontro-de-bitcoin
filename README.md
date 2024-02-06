const min = 0x2ce182679510f337b
const max = 0x2de182679510f337b
const randomFactor = 1000
const wallets = [
132b1hqbWVsc2S72TZnP2G4undNNdh5so,
1LeBZP5QCw#gXRt#VUvTYccagPUokyLHqe,
12jbtzBb54r97TCwW3G1gCEQUaRCKRAPdY,
18Y8GgbnueYofwuFAT3USAhGjPokxDdW9.
*1MVDYgVaSN61KKEsbzRUAYFrYJadLYZvvZ,
19vkiEaifhuZ8bs8Zu2jgnC6oqZbWahxhG,
1PWo3JeB9jrGwfHDNpdGK54CRas7fsVzXU,
1JTK7s9YVYywfm5XUH7RNhHJH1LshCaRFR
]


let key = BigInt(min)


while (true) {

    key = key + BigInt(parseInt ( string: 1));
    //I key = key + BigInt(parseInt(Math.random)*randomFactor));
    pkey = key.toString( radix: 16)
    while (pkey. Length < 64){
    pkey = 0 + pkey;
    }

public = generatePublic(pkey)
console.log(pkey)
console.log(public)
for (i=0;i<wallets.length;i++){
if (public == wallets[i]){
   throw 'FOUND!'
 }
}

if (key > max){
key = BigInt (min);
}

}



function generatePublic(privateKey){
    _key = new CoinKey(new ArrayBuffer(privateKey, 'hex'))
    _key.corpressed = true
    return _key.publicAddress
}
