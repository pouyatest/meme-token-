# meme-token-
transferring meme coin on button click
// Sample script for transferring meme coin on button click
document.getElementById("receiveCoinButton").addEventListener("click", async () => {
  // Call the transfer function of your memecoin contract to send the meme coin to the user's wallet
  // You will need to replace the contract address and function parameters with your actual contract details
  const contractAddress = "YOUR_MEMECOIN_CONTRACT_ADDRESS";
  const amountToSend = 1; // Specify the amount of meme coin to send
  
  // Call the transfer function of the memecoin contract
  await window.ethereum.request({
    method: "eth_sendTransaction",
    params: [{
      to: contractAddress,
      data: 0xa9059cbb000000000000000000000000RECIPIENT_ADDRESS0000000000000000000000000000000000000000000000000000000000000000${amountToSend.toString(16)},
    }],
  });
  
  alert("Meme coin sent successfully!");
});
// this for farcaster platform
