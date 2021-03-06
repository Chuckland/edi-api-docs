AmendmentRequestedEventContent
============================================

.. code-block:: c#

	class AmendmentRequestedEventContent {
		AmendmentRequestMessage: string,
		DiadocBoxId: string,
		InvoiceId: string,
		MessageId: string,
		Torg12Id: string,
		InvoiceCorrectionId: string,
		UniversalTransferDocumentId: string,
		UniversalCorrectionDocumentId: string,
		DiadocUrls: DiadocUrls,
		MessageMeta: BasicMessageMeta,
		UniversalDocumentFunction: UniversalDocumentFunctionType
	}
	
Информация о новом событии в ящике - поступлении уведомления об уточнении документа, сформированного на основании исходящего Invoic. Соответствует BoxEventType = AmendmentRequested.

 - AmendmentRequestMessage – текст уведомления об уточнении,
 - DiadocBoxId – идентификатор ящика в Диадоке, из которого были отправлены подписанные отправителем документы,
 - InvoiceId – идентификатор отправленного счета-фактуры,
 - MessageId – идентификатор сообщения в Диадоке,
 - Torg12Id – идентификатор отправленного ТОРГ-12,
 - InvoiceCorrectionId – идентификатор отправленного корректировочного счета-фактуры,
 - UniversalTransferDocumentId – идентификатор отправленного УПД,
 - UniversalCorrectionDocumentId – идентификатор отправленного УКД,
 - DiadocUrls – :doc:`ссылки на документы в Диадоке <../../structures/DiadocUrls>`,
 - MessageMeta – :doc:`метаинформация <../../structures/BasicMessageMeta>` сообщения Invoic,
 - UniversalDocumentFunction - :doc:`функция УПД <../../enums/UniversalDocumentFunctionType>` сообщения Invoic.