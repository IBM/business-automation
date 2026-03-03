
<div id="media-target" class="video-player"></div>

<style>
	.video-player {
		aspect-ratio: 16/9;
	}
</style>

<script src="https://1.www.s81c.com/common/mediacenter/player/loader/development/loader.js"></script>

<script defer>
	const targetId = 'media-target';
	const uiConfId = '55474022';
	const partnerId = '6010023';
	const entryId = '1_upeu2vuc';

	window?.IBM?.Mediacenter?.player?.embed({
		entryId,
		targetId,
		playerType: video
		partnerId,
		uiConfId,
		environment: 'development',
		autoplay: false
	});
</script>
	