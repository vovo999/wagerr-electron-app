<template>
  <!-- Chain Games Lotto Information Modal -->

  <div id="lotto-info" class="modal modal-fixed-footer bg-gradient">
    <div class="modal-content">
      <div class="row">
        <div class="modal-header">
          <h4>Lotto Information</h4>
        </div>

        <div class="col s12 justified info-text">
          <p>
            The Chain Games lotto has been developed to be provably fair through
            an entropic and fully decentralised selection protocol that can be
            processed by any staking node on the network and validated by every
            other node on the network before being submitted to the blockchain.
          </p>

          <p>
            In short when the lotto payout is triggered, the protocol will add
            together the timestamp and value out of the previous block. Then use
            that sum as an index to loop through the list of entrants to select
            the winner to receive 80% of the pot, 18% is burned and 2% goes to
            the OMN’s.
          </p>

          <p>
            <strong>Number of entrants:</strong> 254

            <br />

            This number is generated by you, the bettors who buy lotto tickets.
          </p>

          <p>
            <strong>Previous block Timestamp:</strong> 1548151033

            <br />

            This number is generated by the blockchain / block time.
          </p>

          <p>
            <strong>Value out of previous block:</strong> 631,700,000,000

            <br />

            This number is generated by the staking selection protocol, the WGR
            holders with balances available for staking and any transaction on
            that block (betting or otherwise).
          </p>

          <p>
            The entrance price is subject to change but is currently 100 WGR.
            Using the numbers above the winner would be entrant 209 and they
            would receive 20,320 WGR.
          </p>
        </div>
      </div>
    </div>

    <div class="modal-footer bg-gradient">
      <div class="options">
        <button class="modal-close waves-effect waves-light btn green">
          Close
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CGLottoInfo'
};
</script>

<style lang="scss" scoped>
.info-text {
  font-size: 1em;
  text-align: justify;
}

.modal-footer {
  display: block;
  background: transparent;
}

.options {
  width: 80px;
  margin-left: auto;
  margin-right: auto;
}
</style>
