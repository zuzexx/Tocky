<script>
	
	import { Accordion, AccordionItem } from 'svelte-collapsible'
	
	const items = [
		{
			key: 'a',
			title: 'One morning, when Gregor Samsa woke from troubled dreams',
			text: 'he found himself transformed in his bed into a horrible vermin. He lay on his armour-like back, and if he lifted his head a little he could see his brown belly, slightly domed and divided by arches into stiff sections. The bedding was hardly able to cover it and seemed ready to slide off any moment'
		},
		{
			key: 'b',
			title: 'Lorem ipsum dolor sit amet, consectetuer adipiscing elit.',
			text: 'Duis leo. Sed fringilla mauris sit amet nibh. Donec sodales sagittis magna. Sed consequat, leo eget bibendum sodales, augue velit cursus nunc,'
		},
		{
			key: 'c',
			title: 'Sed ut perspiciatis unde omnis iste natus error sit voluptatem',
			text: 'similique sunt in culpa qui officia deserunt mollitia animi, id est laborum et dolorum fuga. Et harum quidem rerum facilis est et expedita distinctio. Nam libero tempore, cum soluta nobis est eligendi optio cumque nihil impedit quo minus id quod maxime placeat facere'
		},
        {
			key: 'd',
			title: 'Li Europan lingues es membres de',
			text: ' li pronunciation e li plu commun vocabules. Omnicos directe al desirabilite de un nov lingua franca: On refusa continuar payar custosi traductores. At solmen va esser necessi far uniform grammatica, pronunciation e plu sommun paroles.'
		},
        {
			key: 'e',
			title: 'Quick brown dogs jump over the lazy fox.',
			text: ' Quick brown dogs jump over the lazy fox. The jay, pig, fox, zebra, and my wolves quack! Blowzy red vixens fight for a quick jump. Joaquin Phoenix was gazed by MTV for luck. A wizard’s job is to vex chumps quickly in fog. Watch "Jeopardy!"'
		},
	]
</script>

<div class="acc-container">
    <Accordion>
	
        { #each items as item }
        
            <AccordionItem key={item.key}>
                
                <div slot='header' class='header'>
                    <img src='images/arrow.png' alt="Cover" class="img"/>
                    <div>
                        <h3>{ item.title }</h3>
                        
                    </div>
                </div>
                
                <p slot='body' class='body'>
                    { item.text }
                </p>
    
            </AccordionItem>
        
        { /each }
    
    </Accordion>
    <img src="images/smartphone.png" alt="" class="image">
</div>


<style>
:global(.accordion) {
    width: 30vw;
    max-width: 650px;
    margin: 3rem auto;
}


:global(.accordion-item) {
    border-bottom: 1px solid rgb(100, 120, 140);
}
    .img{
        width: 15px;
        height: 15px;
        margin-top: 1.5rem;
    }
    .image{
        width: 30vw;
        max-width: 650px;
    }
    .header{
        display: flex;
    }
    .acc-container{
        width: 80vw;
        height: auto;
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        text-align: left;
        margin: auto;
    }
    p{
            width: 25vw;
            max-width: 600px;
        }

    @media only screen and (min-width: 1200px) {
       
        .acc-container{
            width: 50vw;
            margin: auto;
        }
    }
</style>