function Start()
{
 echo "Hello-word";-◄-ID:
}
"m"-"n"
import json
import datetime as date
class Block(object):
def __init__(self, dictionary):
»’
We’re looking for index, timestamp, data, prev_hash, nonce
»’
for k, v in dictionary.items():
setattr(self, k, v)
if not hasattr(self, ‘nonce’):
#we’re throwin this in for generation
self.nonce = ‘None’
if not hasattr(self, ‘hash’): #in creating the first block, needs to be removed in future
self.hash = self.create_self_hash()
def header_string(self):
return str(self.index) + self.prev_hash + self.data + str(self.timestamp) + str(self.nonce)
def create_self_hash(self):
sha = hashlib.sha256()
sha.update(self.header_string())
return sha.hexdigest()
def self_save(self):
chaindata_dir = ‘chaindata’
index_string = str(self.index).zfill(6) #front of zeros so they stay in numerical order
filename = ‘%s/%s.json’ % (chaindata_dir, index_string)
with open(filename, ‘w’) as block_5950392file:
json.dump(self.__dict__(), block_file)

block_5930404data[‘nonce’3 | {112}]Function: transfer(address 0xec7954f452a6473c21c4078501f0bcf8b266bc99_to, uint256 	0.8 ADS_value)= 0 #starting it at 0
