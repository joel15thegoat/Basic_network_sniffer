from scapy.all import * 
def packet_sniffer(filter=None) : 
  def process_packet (packet) : 
    if packet.haslayer(IP): 
      src_ip = packet [IP].src 
      dst_ip = packet [IP].dst 
      print(f"Packet from {src_ip} to {dst_ip}") 
    if packet.haslayer(TCP) :  
      src_port = packet [TCP]. sport  
      dst_port = packet [TCP] .dport  
      print (f"TCP Port: {src_port} -> {dst_port}")  
  sniff(filter=filter, prn=process_packet, store=False)   
# Usage  
packet_sniffer("tcp") 
