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
with open(filename, ‘w’) as block_file:
json.dump(self.__dict__(), block_file)

block_data[‘nonce’] = 0 #starting it at 0
